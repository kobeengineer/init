# #純靠北工程師247


Web Extension一直無法replace掉innerText
以為又是被禁止 想了很多方法繞都不行
結果是忘記把replace的結果丟回給自己
靠北


```
td = td.replace(/[零一二三四五六七八九]/g,
function(n) 
return new Array("零","一","二","三","四","五","六","七","八","九").indexOf(n);
);
```


#自我毀滅
