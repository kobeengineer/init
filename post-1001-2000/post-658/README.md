# #純靠北工程師658


有沒有資工系大大可以為我解惑,為什麼小弟用dev_c++寫程式,如圖,單行註解後面的&quot;成功&quot;如果放在最後面的話,程式就無法執行? 這是什麼妖術?還是bug!?


```
#include <cstdlib>
#include <iostream>
#include <cstring>
#include <fstream>
using namespace std;
int main(int argc, char *argv[])
{
      fstream file;// 建立檔案輸出與輸入物件 
      //char buffer[200];
      file.open("sample.txt",ios::out);//開啟檔案
      
      if(file.fail())  //檢查檔案是否開啟成功           
       cout<<"檔案無法開啟\n";
       else
       {
         file<<"編號\t品名\n";
         file<<"A01\t香蕉\n";
         file<<"B01\t鳳梨\n";
         file.close();//關閉檔案  
         cout<<"檔案已建立\n";
        }  
        
        cout<<"press the enter key to continue...";
        cin.get();
        cin.get();
        return EXIT_SUCCESS;
}
```
