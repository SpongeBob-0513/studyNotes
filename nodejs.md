# 简介

![image-20210322212337363](D:\学习文件\笔记OLY\node.js_new\nodejs.assets\image-20210322212337363.png)

![image-20210322225130959](D:\学习文件\笔记OLY\node.js_new\nodejs.assets\image-20210322225130959.png)

# 环境搭建

官网: https://nodejs.org/en/

打开cmd 按照如下输入得到 node.js 的版本，说明安装成功

![image-20210322212743005](D:\学习文件\笔记OLY\node.js_new\nodejs.assets\image-20210322212743005.png)

```javascript
// 引入 http 模块
var http = require('http');

// request: 获取客户端传过来的信息
// response: 给浏览器响应信息
http.createServer(function (request, response) {

    // response.writeHead：设置响应头  
    // 状态码：200
    // 'Content-Type'：编码类型
    response.writeHead(200, { 'Content-Type': 'text/plain' });
    // response.end：表示给页面上面输出一句话并且结束响应
    response.end('Hello World');
}).listen(8081); // 8081：端口

console.log('Server running at http://127.0.0.1:8081/');
```

在 vscode 的终端上运行后，ctrl+c 结束运行

url

**URL 模块** 

![image-20210322222119789](D:\学习文件\笔记OLY\node.js_new\nodejs.assets\image-20210322222119789.png)

# NPM 包管理

+ package.json

在响应文件位置通过 shift + 右键打开power shell     然后输入 npm init 就可以初始化一个

package.json 文件

power shell 里面输入 cls 可以实现清屏

+ npm cnpm

npm init //初始化
npm install xxx //安装
npm i xxx  //简写
npm uninstall xxx//删除
npm un xxx  //简写

cnpm 的服务区在国内，速度比较快

npm update xxx  // 更新
npm install   // 安装 package.json 内已经安装的api
npm i  // 简写

# node 的模块

1. 全局模块 （对象）

   定义:何时何地都能访问，不需要引用

   process.env   环境变量
   process.argv  就是一个数组，可以在里面存储跟访问
   __dirname 目录名

2. 系统模块

   定义:需要require()，但不需要单独下载

   + path:用于处理文件路径和目录路径的实用工具

   ![image-20210323150701678](D:\学习文件\笔记OLY\node.js_new\nodejs.assets\image-20210323150701678.png)

   dirname 打印出来是 /node/a/b/c

   basename       /node/a/b/c     1.jpg

   extname  拓展名字   /node/a/b/c     1.jpg   .jpg

   resolve  可以

   + fs ：用于文件读写操作

     异步方式（大部分是用异步方式）

     ![image-20210323152704587](D:\学习文件\笔记OLY\node.js_new\nodejs.assets\image-20210323152704587.png)

     同步方式

     ![image-20210323152959295](D:\学习文件\笔记OLY\node.js_new\nodejs.assets\image-20210323152959295.png)

   + url 模块

   parse()

3. 自定义模块

   exports   

   ![image-20210323153457362](D:\学习文件\笔记OLY\node.js_new\nodejs.assets\image-20210323153457362.png)

   ![image-20210323153619649](D:\学习文件\笔记OLY\node.js_new\nodejs.assets\image-20210323153619649.png)

如果不加 ./ 会在 node_modules 文件夹下查找 

![image-20210323154017712](D:\学习文件\笔记OLY\node.js_new\nodejs.assets\image-20210323154017712.png)

module

![image-20210323154204742](D:\学习文件\笔记OLY\node.js_new\nodejs.assets\image-20210323154204742.png)

 或者

```javascript
module.exports = function() {
	console.log(123);
}
```

或者

![image-20210323154434706](D:\学习文件\笔记OLY\node.js_new\nodejs.assets\image-20210323154434706.png)

![image-20210323154520802](D:\学习文件\笔记OLY\node.js_new\nodejs.assets\image-20210323154520802.png)

## HTTP 模块

![image-20210323155816296](D:\学习文件\笔记OLY\node.js_new\nodejs.assets\image-20210323155816296.png)

![image-20210323160729661](D:\学习文件\笔记OLY\node.js_new\nodejs.assets\image-20210323160729661.png)

# 数据交互

## GET

![image-20210323165307971](D:\学习文件\笔记OLY\node.js_new\nodejs.assets\image-20210323165307971.png)

![image-20210323164053163](D:\学习文件\笔记OLY\node.js_new\nodejs.assets\image-20210323164053163.png)

![image-20210323164120794](D:\学习文件\笔记OLY\node.js_new\nodejs.assets\image-20210323164120794.png)

## POST

![image-20210323164417408](D:\学习文件\笔记OLY\node.js_new\nodejs.assets\image-20210323164417408.png)

![image-20210323165424328](D:\学习文件\笔记OLY\node.js_new\nodejs.assets\image-20210323165424328.png)

