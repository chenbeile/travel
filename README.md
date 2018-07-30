## 前言
慕课网开源项目实战，本着学习的态度去了解前端，部分问题收集在我的blog里，欢迎浏览
### 预览页面
https://chenbeile.github.io/travel/dist/#/
### 技术栈
vue@2.4 + webpack + node + vue-router + vue-cli + stylus + iconfont + fastclick + vue-awesome-swiper ++ axios + better-scroll + vuex

### 项目运行(进入到travel项目运行)
**安装依赖**  
npm install  
**启动项目**   
npm run dev  
**打开项目**  
localhost:8080


### 项目搭建的过程
使用官方提供的 v-cli 来搭建项目
```
全局安装 vue-cli
$ npm install --global vue-cli  

创建一个基于 webpack 模板的新项目
$ vue init webpack travel  

安装依赖
$ cd travel
$ npm run dev  //启动项目
```
端口: 8080

### 项目上传
```
1. 更新远程代码 ：git pull 
2. git add .
3. git commit -m "注释"
4. 提交本地代码 ：git push 
5. 此项目提交代码的主要步骤  
git checkout -b city-router    //创建并切换到city-router分支  
git add .   //添加city-router分支所有内容  
git commit -m  'city路由配置'  //注释  
git push --set-upstream origin city-router   //提交city-router分支内容  
git chekout master  //切换到主分支  
git merge city-router   // 合并刚才改的分支  
git push  // 再提交主分支  

git关于分支的其他操作浏览阮一峰大神的blog(http://www.ruanyifeng.com/blog/2014/06/git_remote.html)  
```
### 项目效果图
![travel效果图](./travel.gif)  

项目功能简单，但涵盖了vue大部分的知识点, 适合入门学习

### 交流
如觉得有帮助，star一下？
欢迎加QQ524443229交流问题

 
