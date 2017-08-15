# #純靠北工程師3bd


...


```
var user=new User('devilcancry')
user.getPosts().then(posts=>{
	posts.forEach(post=>{
		var content=post.content
		if(content.includes('幹大事')&&content.includes('阿拉花瓜')){
			new User('lolimaple').report(user)
		}
	})
})
```
