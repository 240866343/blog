---
title: Nodejs简述
---
### 1. Nodejs是什么？
-  首先需要明白Nodejs不是一个js应用、而是一个js运行平台。其是由C++编写而成。但是Nodejs是一个后端的运行环境。因此你可以编写系统级或者服务器端的js让Nodejs帮你执行。
- nodeJS,是可以运行在后端的JavaScript。
- 为什么它能够在后端运行呢？
- 这就得归功于V8引擎（V8是Google Chrome浏览器的JavaScript引擎），通过对高性能V8引擎的封装，并通过一系列优化的API类库，使其就能够在后端运行了。
- JavaScript是单线程，所以要做到无阻塞，node是通过大量的回调函数来达到这一目的。

### 2.并且Nodejs有两大特点：

- 基于事件驱动；
- 无阻塞。
### 3.安装nodejs

- 首先到官网下载
More info:[nodeJS](https://link.jianshu.com/?t=https://nodejs.org/)
- 在下载完安装包后，在windows下按照默认程序走就ok啦
- 检验是否安装成功，在Windows环境下，打开命令提示符，输入node – v
![image.png](http://upload-images.jianshu.io/upload_images/9246752-4f085c8bc724a8b1.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


- npm在你安装nodeJS时，就一带帮你安装了。打开命令提示符，输入npm – v
![image.png](http://upload-images.jianshu.io/upload_images/9246752-8ad6893b69b79d32.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)



- 在命令提示符下，敲打我们的程序，你只需输入node，然后回车就可以进入node在命令提示符下的交互环境了。
![image.png](http://upload-images.jianshu.io/upload_images/9246752-cd4bf8722cadcb37.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


- 进入node交互环境后，敲到"hello world"字符串后回车。
![image.png](http://upload-images.jianshu.io/upload_images/9246752-4f961a5a8b2e5e86.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

- 如果你想退出node的这个交互环境，就Ctrl + C，连按两次就退出回到windows命令符啦。






### 4.接下来我们就用nodeJS来开发一个最简单的服务器程序。

![image.png](http://upload-images.jianshu.io/upload_images/9246752-af0b87e55ef29893.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


![image.png](http://upload-images.jianshu.io/upload_images/9246752-1ff740d9204dbde7.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


### 接下来赶快去探索你的Nodejs吧，少年！