# #純靠北工程師3c0


今天重構看到的&quot;前輩&quot;程式碼


```
bool selected;
if(selected==true)
  ...
else if(selected==false)
  ...
...

Map filter={
  ...
}
if(option=="option1")
  filter["option"] = "option1"
else if(option=="option2")
  filter["oprion"] = "option2"
...

```
