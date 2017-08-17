# #純靠北工程師512


關於今日的我


```
public class Main{
    static School school;
    public static void main(String[] argv){
        school = School.getInstance();
        final Me me = Me.builder()
                  .sex(Sex.BOY)
                  .dick(30).cm()
                  .condom(null)
                  .born();
        me.setOnFuckListener(new FuckAndKillTheChild()){
            public void onChildBorn(Child child){
                me.kill(child);
            }
        }
        for (Woman woman : school.girls)
            try{
                me.fuck(woman);
            }catch(ClimaxException err){
                err.shootOnHerFace(woman);
            }

    }
}

```
