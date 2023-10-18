## 前后端分离项目模版

### 如何跑通 ⭐

- 第一步拉取代码
- 第二步前端执行命令安装依赖
- 第三步后端找到配置文件修改为自己的配置
- 第四步修改前端访问接口
- 第五步浏览器地址栏输入地址进行访问
- 进行注册，使用

### 技术栈 ⭐
- 前端：vue 3 ⭐
- 后端：spring boot 2.x、MySQL 🌟
- test: 🐔

包含基本的登录、注册、密码重置等等功能，可以二次开发编写具体场景下的应用程序。

* 登录功能（支持用户名、邮箱登录）🌟
* 注册用户（通过邮箱注册）⭐
* 重置密码（通过邮箱重置密码）

登录功能：
1. 用户登录成之后，才能访问index路径下的页面
2. 用户如果没有登录，那么会自动跳转到登录界面
3. 如果用户请求的是一个压根就不存在的页面，依然强制回到登录界面，如果已经登录，那么回到index首页

登录解决方案
1. 无论是否已经登录，直接向后端请求用户信息
2. 如果请求成功，那么说明肯定是已经登录了
3. 如果请求失败，那么说明没有登录，跳转到登录界面
