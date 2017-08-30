# #純靠北工程師78f


網路上找到的動態二維陣列宣告...
有人知道運作原理嗎



```
void* New2d(int h, int w, int size){
	void **p;
	p = (void**)new char[h * sizeof(void*) + h*w*size];
	for (int i = 0; i ＜h; i++)
		p[i] = ((char *)(p + h)) + i*w*size;
	return p;
}
```
