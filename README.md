# Wechat App 
## dickson's branch
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




#### 2.注册小程序页面，了解一些常用标签
1.第一个示例中的小程序主要用到了<view></view>和<text></text>,这两个标签应该类似web开发中的块级元素div和p，有一个需要注意的地方就是只有用<text></text>包裹起来的元素才能有触发长按选中文字功能
#### 3.一些CSS的知识：Flex盒子以及移动端自适应的概念
1.rpx：移动端各种设备的像素不一样（比如一个头像，应该按照一定比例在iphone4和iphone6中显示，而不是用一种尺寸在两种设备中显示），我们需要动态去适应不同分辨率的设备，在移动端的页面开发中很少会用逻辑像素px，小程序用rpx来做自适应，2rpx = 1px，让ui以iphone6（宽750px）的尺寸来设计效果图，这样就可以按照1比1来换算。
总结就是如果拿的是宽度750像素的设计图直接可以直接按照1比1的关系来换算。


