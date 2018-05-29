# vue-review
独立开发一个vue项目

进入现在的公司后，公司所有开发的项目都是用vue，之前架构方面都是老大弄的，为了证明我也可以，我按照自己的方法在重新弄了一下。下面是我的经验总结：

一、搭建VUE脚手架： https://github.com/vuejs-templates/webpack 
$ npm install -g vue-cli
$ vue init webpack my-project
$ cd my-project
$ npm install
$ npm run dev

二、关于平台其它插件使用：
平台的UI框架是element-ui,之前平台是用的element-ui的1.3.7的版本，这个版本太老了，所以我选的是2.3.9：http://element-cn.eleme.io/2.3/#/zh-CN/component/quickstart

平台路由是学习router-link:https://router.vuejs.org/zh/

平台接口调用是用axios,虚拟接口数据是用mock.js

平台字体是用的font awesome 和 normalize.css:npm i font-awesome 和 npm i normalize.css

在平台中，js部分我尽量用ES6：http://es6.ruanyifeng.com/#docs/array

平台打包是用的webpack：https://www.webpackjs.com/

平台的样式风格是参照的腾讯云。

三、目录结构
之前老大架构的项目目录结构我觉得很好，但是他是针对大型网站做的，我这个项目只是一个小的demo，不需要做的那么复杂，所以在目录结构上，我根据自己的需求弄得简单些：

|-- build             -- 构建目录
|-- config            -- 构建配置目录
|-- src               -- 项目源文件
   |-- assets         -- 项目js、css、img资源
   |-- components 
       |-- common     -- 项目公共模块(顶部、常用服务列表、左边导航栏、小模块导航栏)
       |-- module
           |-- module1
               |-- div1
                   ...
               |-- divn
               |-- router
               ...
           |-- module n
           |-- router
|-- static            -- 项目静态资源目录
|-- index.html        -- 项目初始页面

四、项目开发中遇到的难点

1、首页全屏问题：
首页因为是全屏，所以首页各个模块都必须要计算出来，让每个模块在大小屏中都能正常显示







