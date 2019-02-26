# Wechat App 
## maomao's branch
Learn how to develop wechat app

### 前期准备
##### 1.申请小程序账号
暂时先不用AppID，可先不申请

##### 2.下载或克隆项目源码
https://developers.weixin.qq.com/miniprogram/dev/devtools/download.html

##### 3.新建小程序项目
下载完开发工具后安装点击新建小程序，AppID暂时选测试，后台不选，创建完后生成这个界面：
<img src="https://raw.githubusercontent.com/taotao820/md-images/master/wechat-app/Screenshot/gotoMain.jpg" alt="">


#### 4.了解一些小程序开发特性
及时编译
调试代码：如图：<img src="https://raw.githubusercontent.com/taotao820/md-images/master/wechat-app/Screenshot/console.jpg" alt="console.jpg">（小程序的调试工具用的就是chrome的控制台，调试技巧具体开发的时候我跟你们说）
blabla 到这是前两章的内容，视频基本可以不看了


### 编写第一个小程序
#### 1.小程序文件类型和目录结构
新建一个ReadAndMovie项目
(1)web project主要包含.css html .js这三种类型文件，.json一般放一些数据配置或者前端自测联调后台接口的数据
一般新建一个项目后的文件目录是这样的：
```js
+-- pages/                                  ---核心代码目录
|   +-- index                               
|   |    --- index.js                       ---js文件 对应web应用中的js文件
|   |    --- index.json                     ---对应web应用中的json文件，配置文件
|   |    --- index.wxss                     ---对应web应用中的css文件，样式文件
|   +-- logs                                ---日志文件夹
+-- utils/                                  ---核心代码目录
|   --- utils                               ---公共工具方法   
--- app.js                                  ---app应用入口文件，不可修改只有一个
--- app.json
--- app.wxss
--- project.config.json              
```
第一个小程序可以删掉一些文件夹，目录如图：


#### 2.注册小程序页面，了解组件基本用法
#### 3.一些CSS的知识：Flex盒子以及移动端自适应的概念

