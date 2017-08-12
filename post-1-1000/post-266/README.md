# #純靠北工程師266


...


```
class Human extends Living{
  //define some fields......
  private Human companion;
  public Human getCompanion(){
    return this.companion;
  }
  public void setCompanion(Human cp){
    this.companion=cp;
  }
}
class Engineer extends Living{
  //define some other fields......
  @Override
  public void setCompanion(Human cp){
    this.companion=null;
  }
}
```
