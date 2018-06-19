# 功能：
使用Python的Selenium包爬取特定新浪微博用户的信息

# 说明：
爬取内容：爬取用户ID 用户名 粉丝数 关注数 微博数 性别 所在地 个人简介 微博内容 用户头像 \<br>
数据保存：个人信息、微博文本保存到数据库和本地csv 头像保存到本地
网址：微博手机版 www.weibo.cn

# 步骤：
1.调用界面浏览的浏览器Firefox访问微博手机版网页
2.使用账号和密码登录微博（预留时间，需要手动输入验证码）
3.从数据库读取需要爬取的用户id
4.逐一访问用户：
  4.1.爬取【用户主页】的【昵称、粉丝数、关注数、微博数、头像文件地址】，并下载头像图片至本地
  4.2.爬取【用户资料页】的【性别、所在地、个人简介】
  4.3.爬取【用户微博】
