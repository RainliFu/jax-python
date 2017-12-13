# flask-demo
个人Flask练手项目，以pycon2014上miguel的项目为基础进行改编,实现了一个简易的
微博客,具有注册、登录、发博客、关注、评论等功能.
###使用说明

1. git clone https://github.com/goalong/flask-demo.git
2. cd flask-demo
3. virtualenv venv
4. source venv/bin/activate
5. pip install -r requirements.txt
6. python manage.py runserver
7. 打开浏览器，在地址栏输入http://localhost:5000/
8. 注册用户，在终端输入 python manage.py adduser <email> <username> 

###Todo
1.文章的收藏 delay
2.文章的喜欢或者赞同, 赞同应该不近包括文章,还可以对评论,以及可能的其他对象
3.文章加标签
4.迁移python3
5.迁移使用mysql
6.第三方依赖升级， 已完成
7.消息，如被关注会有消息，被点赞会有消息
8. 重新设计comment，允许回复评论, 滚动到哪个评论才会在哪个评论那里出现回复的入口,参考果库的评论设计，评论的点赞和回复
9. 改版评论,评论应该作为社区的主题予以重视,参考v站的形式,不分父评论和子评论,扁平化,所有评论是平行的平等的,
10, 赞同按钮点击之后变色,再点击恢复,参考果库图文,优先级不高

加一个标签的列表页
应用一个所见即所得的编辑器  重要


给每一个评论一个特定的URL,方便跳转到

###Finish
评论扁平排版
评论的点赞
文章的评论以及对评论的回复已经搞定,
审查一下原来的关注及取关的表结构的模型,看看有没有问题,现在的需要改进,因为自己都看不懂了
加了标签,还需要一个标签展示页面

可以设计一个如同豆瓣的豆单那种的功能,一个聚合同类型对象的列表


其实user_approve这个表应该拆分出几种(因为这个表的记录增长会很快),对文章的赞同是一个表,对评论的赞同是一个表,

接下来重点: 加标签 加消息通知

类似知乎的组织方式