# #純靠北工程師1b3


洗讚前端腳本
先一直往下滑 把文章都載入
然後按ctrl + shift + c 
點console
再把這些貼上

var L = document.getElementsByClassName(&quot;UFILikeLink&quot;);rrrri = 0;function doSomething(){if(rrrri == 0){alert(&quot;總共有&quot; + (L.length + 1) + &quot;個讚\n約需花&quot; + (L.length + 1) * 2.5 + &quot;秒&quot;);}if(rrrri &lt; L.length){L[rrrri].click();console.log(&quot;第&quot; + (rrrri + 1) + &quot;個讚&quot;);rrrri++; setTimeout(doSomething,2500);}else{alert(&quot;完成&quot;);}}doSomething();


```
var L = document.getElementsByClassName("UFILikeLink");
rrrri = 0;
function doSomething(){
	if(rrrri == 0){
		alert("總共有" + (L.length + 1) + "個讚\n約需花" + (L.length + 1) * 2.5 + "秒");
	}
	if(rrrri < L.length){
		L[rrrri].click();
		console.log("第" + (rrrri + 1) + "個讚");
		rrrri++; 
		setTimeout(doSomething,2500);
	}
	else{
		alert("完成");
	}
}
doSomething();
```


#屁孩也會寫程式
