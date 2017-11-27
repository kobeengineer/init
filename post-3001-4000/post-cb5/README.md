# #純靠北工程師cb5



UPDATE wp_sizx_posts 
SET wp_sizx_posts.post_status = &#039;trash&#039; 
FROM wp_sizx_posts
	INNER JOIN wp_sizx_post_views
	ON wp_sizx_posts.ID=wp_sizx_post_views.id
WHERE wp_sizx_post_views.count=&#039;0&#039;;

MySQL 回應: 說明文件

#1064 - You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near &#039;FROM wp_sizx_posts
    INNER JOIN wp_sizx_post_views
    ON wp_sizx_posts.ID=wp_sizx&#039; at line 3 
求解
