# #純靠北工程師6c7


除錯信息:Error (10476): VHDL error at tsl2561_basys_example.vhd(198): type of identifier &quot;tsl2561_interface&quot; does not agree with its usage as &quot;entity&quot; type
怎改..新手..拜託各位大神


```

library ieee;
use ieee.std_logic_1164.all;

entity tsl2561_basys_example is

  port(
    clk   : in std_logic;
    reset : in std_logic := '0';
    sda : inout std_logic;
    scl : inout std_logic;
    seg : out std_logic_vector(6 downto 0);
    an  : out std_logic_vector(3 downto 0)

  );

end tsl2561_basys_example;

architecture Behavioral of tsl2561_basys_example is
component tsl2561_interface is

  generic(

    address : std_logic_vector(6 downto 0) := "0111001";

    clk_frequency : integer := 50_000_000;

    i2c_frequency : integer := 100_000

  );

  port(

    clk   : in std_logic;

    reset : in std_logic := '0';

    sda : inout std_logic;

    scl : inout std_logic;

    light_intensity : out std_logic_vector(15 downto 0)

  );

end component tsl2561_interface;

  signal light_intensity : std_logic_vector(15 downto 0);

begin


  SENSOR_INTERFACE:

  entity tsl2561_interface generic map(

    address => "0111001",


    clk_frequency => 50_000_000,


    i2c_frequency => 100_000

  )

  port map(

    clk             => clk,

    reset           => reset,

    sda             => sda,

    scl             => scl,

    light_intensity => light_intensity

  );

  SSEG_DISPLAY_DRIVER:

  entity sseg_driver port map(

    clk          => clk,

    leftmost     => light_intensity(15 downto 12),

    left_center  => light_intensity(11 downto 8),

    right_center => light_intensity(7 downto 4),

    rightmost    => light_intensity(3 downto 0),

    cathodes     => seg,

    anodes       => an

  );



end Behavioral;
```
