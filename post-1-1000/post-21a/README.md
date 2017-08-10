# #純靠北工程師21a


RE: #純靠北工程師207
如果用.NET語言（C#|vb.net）做模擬器，該怎樣
1. 繪製圖片（DrawImage）和
2. 更新畫面（Paint Event還是設定BackgroundImage）比較好？
3. 需要 Doublebuffered 和
4. Timer 嗎？
5. 還有如何釋放用完的New Bitmap()記憶體，將Frame變回空白圖(
應該不是frame = new Bitmap(...);吧
還是
Dim a as new Bitmap(...)
6. &#039;這個跟 Dim a as Bitmap = new Bitmap(...);/Bitmap a = new Bitmap(...); 有差嗎？
frame = a;
a.dispose;
還是
Using a as new bitmap(...)
 frame = a;
end using
)
，否則一段時間後就會記憶體不足？
7. 還有FPS(frame per second)的定義是最近一秒畫格數、1除一畫格所需時間、還是累積畫格數除秒數？
8. 當設定Me.backgroundimage = frame （Global 變數）時，frame有改變背景也會跟著改變的情況好嗎？
