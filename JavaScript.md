#  JavaScript 是什么

+ JavaScript 是世界上最流行的语言之一，是一种运行在**客户端**的**脚本语言** （Script 是脚本的意思）

+  脚本语言：不需要编译，运行过程中由 js 解释器( js 引擎）逐行来进行解释并执行

+ 现在也可以基于 Node.js 技术进行服务器端编程

 **JavaScript的作用**
表单动态校验（密码强度检测)(JS产生最初的目的)

网页特效

服务端开发(Node.js)

桌面程序(Electron)

App(Cordova)

控制硬件-物联网(Ruff)

游戏开发(cocos2d-js)

![image-20210308222801539](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210308222801539.png)

![image-20210308223245459](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210308223245459.png)

# JS 的组成

![image-20210311174800616](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311174800616.png)

![image-20210308223551256](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210308223551256.png)

![image-20210308223639812](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210308223639812.png)

![image-20210308223708538](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210308223708538.png)

+ 三种写法

行内式    内嵌式    外部 JS 文件

![image-20210309143355678](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309143355678.png)

注意单双引号的使用: 在HTML中我们推荐使用**双引号**,JS中我们推荐使用**单引号**

# 输入输出语句

![image-20210309144420076](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309144420076.png)

# 变量

1. 声明变量
2. 赋值

![image-20210309145216121](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309145216121.png)

![image-20210309151400318](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309151400318.png)

命名规范

![image-20210309151740174](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309151740174.png)

尽量不要使用 name ，因为有些浏览器中定义了 name

# 数据类型

js 的变量数据类型是只有程序在运行过程中，根据等号右边的值来确定的

## 简单数据类型

![image-20210309154346401](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309154346401.png)

+ **Number**

![image-20210309154854343](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309154854343.png)

```javascript
// 1．数字型的最大值
console.log(Number.MAX_VALUE);
// 2．数字型的最小值
console.log(Number.MIN_VALUE);
// 3．无穷大
console.log(Number.MAX_VALUE * 2); // Infinity无穷大
// 4．无穷小
console.log( -Number.MAX_VALUE * 2); // -Infinity 无穷大

```

NaN     ,Not a number ，代表一个非数值

 **isNaN()** 这个方法用来判断非数字，并且返回一个值如果是数字返回的是 false ，如果不是数字返回的是true

+ **String**

![image-20210309155901943](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309155901943.png)

  转义符

![image-20210309160031973](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309160031973.png)

length属性 

![image-20210309160911907](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309160911907.png)

字符串拼接

![image-20210309161251547](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309161251547.png)

+ **布尔型 Boolean**

true  false

![image-20210309161753188](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309161753188.png)

+ **Undefined 和 Null**

![image-20210309162046608](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309162046608.png)

## 获取数据类型

![image-20210309162410130](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309162410130.png)

## 数据类型转换

转为字符串

![image-20210309162910234](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309162910234.png)

转为数字型

![image-20210309163517110](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309163517110.png)

![image-20210309163329083](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309163329083.png)

转换为布尔型

![image-20210309184909810](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309184909810.png)

解释型语言 和 编译型语言

![image-20210309185307022](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309185307022.png)

+ 算数运算符

![image-20210309191310538](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309191310538.png)

![image-20210309191925023](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309191925023.png)

+ 递增和递减运算符

++   --

前置：先自加 ，后返回值

后置：先返回原值，后自加

![image-20210309192319851](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309192319851.png)

+ 比较运算符

![image-20210309193040183](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309193040183.png)

默认转换数据类型会把字符串型的数据转换为数字型

+ 逻辑运算符

![image-20210309193258278](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309193258278.png)

短路运算

![image-20210309195925533](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309195925533.png)

![image-20210309200112728](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309200112728.png)

+ 赋值运算符

![image-20210309200219092](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309200219092.png)

+ 运算符优先级

![image-20210309200414838](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309200414838.png)

# 流程控制

 ## 顺序流程控制

​       顺序结构是程序中最简单、最基本的流程控制，它没有特定的语法结构，程序会按照代码的先后顺序，依次执行，程序中大多数的代码都是这样执行的。

## 分支流程控制

if 分支结构

![image-20210309203501606](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309203501606.png)

![image-20210309204512547](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309204512547.png)

![image-20210309204717485](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309204717485.png)

三元表达式

![image-20210309205049964](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309205049964.png)

switch 语句

![image-20210309205350638](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309205350638.png)

要求**全等**，必须是值和数据类型一致才可以

## 循环流程结构

for循环

![image-20210309210446265](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309210446265.png)

双重for循环
while循环
do while循环
continue, break

# 断点调试

![image-20210309210743541](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309210743541.png)

# 数组

## 创建数组

![image-20210309212531432](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309212531432.png)

![image-20210309212620425](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309212620425.png)

![image-20210310214556086](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310214556086.png)

## 访问数组元素

![image-20210309212909014](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309212909014.png)

# 函数

1. 声明函数

   方法一：命名函数

   ![image-20210309214431273](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309214431273.png)

   方法二： 函数表达式（匿名函数）

   ![image-20210309222203984](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309222203984.png)

   该方法中的 fun 才是变量名，其中的函数没有名字，称为变量名。

   该函数表达式声明方式跟声明变量差不多，只不过变量里面存的是值而函数表达式里面存的是函数。

   ```javascript
   input.select();  //文本框里面的文字处于选定状态
   ```

   方法三： new Function()  (了解)

   ![image-20210320193511786](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320193511786.png)

   + 函数也属于对象

   ![image-20210320193808579](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320193808579.png)

2. 调用函数

   函数名();

![image-20210309215002156](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309215002156.png)

**注意：**如果函数没有返回值，则返回undefined

## 函数调用方式

![image-20210320193942029](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320193942029.png)

1.普通函数

![image-20210320194028482](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320194028482.png)

2.对象的方法

![image-20210320194119428](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320194119428.png)

3.构造函数

```javascript
function Star() {};
new Star();
```

4.绑定事件函数

```javascript
btn.onclick() = function() {}; //点击按钮就可以调用这个函数
```

5.定时器调用

```javascript
setInterval(function() {}, 1000); //这个函数是自动 1 秒钟调用一次
```

6.立即执行函数

```javascript
(funtion() {
 		console.log('人生的巅峰')；
})
```

## 函数 this 的指向

![image-20210320195025375](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320195025375.png)

## 改变函数内部 this 指向

+ call()

![image-20210320215334318](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320215334318.png)

```javascript
<script>
        //改变函数内this指向js提供了三种方法 call() apply() bind()
        // 1. call()
        var o = {
            name: 'andy'
        }
        function fn(a, b) {
            console.log(this); console.log(a + b);
        };
        fn.call(o, 1, 2);
        // call第一个可以调用函数第二个可以改变函数内的this指向
        // call的主要作用可以实现继承
        function Father(uname, age, sex) {
            this.uname = uname;
            this.age = age;
            this.sex = sex;
        }
        function Son(uname, age, sex) {
            Father.call(this, uname, age, sex);
        }
        var son = new Son('刘德华', 18, '男');
        console.log(son);
    </script>
```

+ apply()

![image-20210320215530793](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320215530793.png)

```javascript
<script>
        // 2. apply()应用运用的意思
        var o = {
            name: 'andy'
        };
        function fn(arr) {
            console.log(this);
            console.log(arr);  // 'pink'
        };
        fn.apply(o, ['pink']);
        // 1．也是调用函数第二个可以改变函数内部的this指向
        // 2．但是他的参数必须是数组(伪数组)
        // 3. apply 的主要应用 比如说我们可以利用apply 借助于数学内置对象求最大值
        // Math.max();
        var arr = [1, 66, 3, 99, 4];
        var arr1 = ['red', 'pink'];
        // var max = Math.max.apply(null,arr);
        var max = Math.max.apply(Math, arr); 
        var min = Math.min.apply(Math, arr); 
        console.log(max, min);
    </script>
```

+ bind()    bind 是捆绑的意思

![image-20210320220902359](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320220902359.png)

```javascript
 <script>
    <button>点击</button>
    <script>
        // 3.bind(）绑定捆绑的意思
        var o = {
            name: 'andy'
        };
        function fn(a, b) {
            console.log(this);
            console.log(a + b);
        };
        var f = fn.bind(o, 1, 2);
        f();
        // 1．不会调用原来的函数可以改变原来函数内部的this 指向
        // 2．返回的是原函数改变this之后产生的新函数
        // 3. 如果有的函数我们不需要立即调用,但是又想改变这个函数内部的this指向此时用bind
        // 4．我们有一个按钮,当我们点击了之后,就禁用这个按钮,3秒钟之后开启这个按钮
        var btn1 = document.querySelector('button');
        btn1.onclick = function () {
            this.disabled = true;//这个this指向的是 btn这个按钮 
            //var that = this;
            setTimeout(function () {
                // that.disabled = false; //定时器函数里面的this 指向的是window
                this.disabled = false; //此时定时器函数里面的this指向的是btn
            }.bind(this), 3000); //这个this指向的是btn这个对象
        }

    </script>
```

![image-20210320223025700](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320223025700.png)

## arguments

所有函数都内置了一个arguments对象，arguments对象中存储了传递的所有实参。

伪数组：

![image-20210309221316646](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309221316646.png)

伪数组：

![image-20210309221123879](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309221123879.png)

![image-20210310204433405](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310204433405.png)

# 作用域

全局作用域   局部作用域

![image-20210309222945975](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210309222945975.png)

**1．** **全局变量**:在全局作用域下的变量在全局下都可以使用

**注意**：如果在函数内部没有声明直接赋值的变量也属于全局变量

**2．** **局部变量**：在局部作用域下的变量

**注意**：函数的形参也可以看作局部变量

**3．**从执行效率来看全局变量和局部变量

(1）全局变量只有浏览器关闭的时候才会销毁，比较占内存资源

(2)局部变量当我们程序执行完毕就会销毁，比较节约内存资源

**作用域链**

内部函数可以用外部函数的变量，采取**就近原则**（也称作链式查找）

# JavaScript 预解析

JavaScript代码是由浏览器中的JavaScript解析器来执行的。JavaScript解析器在运行JavaScript代码的时候分为两步∶**预解析**和**代码执行**。

预解析 js引擎会把js里面所有的 var 还有 function提升到当前作用域的最前面

![image-20210310091431868](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310091431868.png)

案例

![image-20210310094608527](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310094608527.png)

# 对象

由属性和方法组成

![image-20210310190434479](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310190434479.png)

**创建对象的三种方式**

1. **利用字面量创建对象**

![image-20210310191500883](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310191500883.png)

![image-20210310191533351](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310191533351.png)

对象的调用

![image-20210310191637474](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310191637474.png)

![image-20210310192449450](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310192449450.png)

2. **利用new Object创建对象**

![image-20210310192851328](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310192851328.png)

3. **利用构造函数创建对象**

**构造函数**就是把我们对象里面一些相同的属性和方法抽象出来封装到函数里面

1. 构造函数名字的首字母要大写
2. 我们构造函数不需要return就可以返回结果
3. 我们调用构造函数必须使用new
4. 我们只要new Star()调用函数就创建一个对象ldh {}
5. 我们的属性和方法前面必须添加this T

![image-20210310200941611](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310200941611.png)

new 关键字的四部曲

![image-20210310202331663](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310202331663.png)

## 遍历对象

for  in

![image-20210310202940872](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310202940872.png)

## 内置对象

内置对象就是指 JS 语言自带的一些对象，这些对象供开发者使用，并提供了一些常用的或是最基本而必要的功能(属性和方法)

JavaScript 提供了多个内置对象: Math、 Date 、Array、String等。

### **Math 对象**

![image-20210310204623722](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310204623722.png)

![image-20210310204720763](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310204720763.png)

![image-20210310205303446](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310205303446.png)

random()

![image-20210310205941265](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310205941265.png)

其余的看文档

### **日期对象**

date （构造函数 选哟 new 一个）

![image-20210310210942974](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310210942974.png)

日期格式化

![image-20210310211347746](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310211347746.png)

获得总的毫秒数（永远都不会重复的，也叫 **时间戳**）

![image-20210310212212618](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310212212618.png)

### **数组对象**

![image-20210310214602227](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310214602227.png)

检测是否为数组

instanceof     isArray()

![image-20210310215007090](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310215007090.png)

添加删除数组元素的方法

push()  pop()  unshift()   shift()

![image-20210310215229746](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310215229746.png)

数组排序

reverse()  sort()

![image-20210310215554681](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310215554681.png)

![image-20210310220417598](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310220417598.png)

数组索引方法

indexOf()  lastIndexof()

![image-20210310220502770](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310220502770.png)

数组转换为字符串

toString()  join()

![image-20210310220913930](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310220913930.png)

其他

concat()  slice()  splice()

![image-20210310221019890](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210310221019890.png)

### 字符串对象

字符串类型是基本数据类型，本来是没有属性和方法的，但是 js 把它包装成为了复杂数据类型，从而有了复杂数据类型的性质。

基本包装类型

![image-20210311145440105](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311145440105.png)

根据字符返回位置

indexOf()   lastIndexOf()

![image-20210311145921097](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311145921097.png)

根据位置返回字符

charAt()  charCodeAt()  str[]

![image-20210311150424360](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311150424360.png)

字符串的操作方法

concat()  substr() slice()  substring()

![image-20210311152421203](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311152421203.png)

其他方法

replace()  split()

![image-20210311160620068](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311160620068.png)

![image-20210311160704888](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311160704888.png)

toUpperCase()  toLowerCase()

![image-20210311160736199](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311160736199.png)

# 简单数据类型和复杂数据类型

![image-20210311161145492](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311161145492.png)

null 比较特殊

![image-20210311161114135](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311161114135.png)

## 堆和栈

![image-20210311161553507](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311161553507.png)

![image-20210311161634881](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311161634881.png)

![image-20210311161749875](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311161749875.png)

## 简单类型传参

![image-20210311172955199](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311172955199.png)

上图中的输出 x 还是 10，不会受函数内部的影响

## 复杂类型传参

![image-20210311173728203](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311173728203.png)

![image-20210311173936823](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311173936823.png)

# Web APls

API

![image-20210311175452683](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311175452683.png)

Web API

![image-20210311175624611](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311175624611.png)

https://developer.mozilla.org/zh-CN/docs/Web/API

## DOM

### 简介

**文档对象模型**( Document Object Model，简称DOM)，是W3C组织推荐的处理可扩展标记语言（HTML或者XML)的标准编程**接口**。
W3C已经定义了一系列的DOM接口，通过这些DOM接口可以改变网页的内容、结构和样式。

![image-20210311180725118](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311180725118.png)

**文档 ** : 一个页面就是一个文档，DOM中使用**documen**t表示
**元素** : 页面中的所有标签都是元素，DOM中使用**element**表示
**节点**∶网页中的所有内容都是节点（标签、属性、文本、注释等），DOM中使用**node**表示

==DOM把以上内容都看做是对象==

### 获取元素

![image-20210311181245757](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311181245757.png)

JavaScript 书写位置

![image-20210311181549271](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311181549271.png)

console.dir  (下面举例中的time 是 timer 的 id，没有写错)

![image-20210311182106397](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311182106397.png)

![image-20210311182159802](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311182159802.png)

+ 根据ID获取
  使用 getElementByld()  方法可以获取带有ID的元素对象。

​       其中 参数 id 是大小写敏感的**字符串**

​       返回的是一个元素**对象**

+ 根据标签名获取
  使用 getElementsByTagName() 方法可以返回带有指定标签名的对象的集合。（集合所以要加 s）

  **返回**的是获取过来元素对象的集合以**伪数组**的形式存储的

  ![image-20210311183608821](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311183608821.png)

  ![image-20210311183936127](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311183936127.png)

​              用上面的方法之前首先应该获得父元素对象，并且父元素必须是指定的单个元素

+ 通过HTML5新增的方法获取

1. document.getElementsByClassName( '类名' );//根据类名返回元素对象集合
2. document.queryselector ( '选择器'); //根据指定选择器返回第一个元素对象 （选择器就是css 里面的选择器 例如 .nav等）
3. document.querySelectorAll('选择器');//根据指定选择器返回

+ 获取特殊元素(body , html )
  **获取body元素**

1. ```javascript
  doucument.body  //返回body元素对象
  ```


  **获取html元素**

2. ```javascript
   document.documentElement  //返回html元素对象
   ```

### 事件  基础

事件三要素： 事件源  事件类型  事件处理程序

![image-20210311195642294](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311195642294.png)

![image-20210311195915664](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311195915664.png)

![image-20210311195936296](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311195936296.png)

**常见的鼠标事件**

![image-20210311200017692](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311200017692.png)

双击事件是:  **ondblclick**

如果双击文字,会默认选定文字,此时需要双击禁止选中文字
window.getSelection ? window.getSelection().removeAllRanges() : document.selection.empty();

![image-20210313165710970](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210313165710970.png)

事件

获得焦点 onfocus

失去焦点 onblur

当复选框发生改变的时候 change事件   

![image-20210311222910543](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311222910543.png)

==注意== 如果是手动调用事件，就不需要写 on

例如:

![image-20210320090901460](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320090901460.png)

### 事件 高级

+ 注册事件概述
  给元素添加事件，称为注册事件或者绑定事件。
  注册事件有两种方式∶传统方式和方法监听注册方式

  1. **传统注册方式**
     利用on开头的事件onclick

  ```javascript
  <button onclick= "alert('hi~")”></button>
  btn.onclick = function)(){}
  ```

  特点: 注册事件的**唯一性**

  同一个元素同一个事件只能设置一个处理函数，最后注册的处理函数将会覆盖前面注册的处理函数

  2. **方法监听注册方式**
     w3c标准推荐方式
     addEventListener()它是一个方法，IE9之前的E不支持此方法，可使用attachEvent()代替特点∶同一个元素同一个事件可以注册多个监听器(监听器就是监听处理函数)

     按注册顺序依次执行

     ![image-20210313134425426](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210313134425426.png)

     ![image-20210313135241316](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210313135241316.png)

     ![image-20210313135428430](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210313135428430.png)

     删除事件

     ![image-20210313140128965](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210313140128965.png)

​             ![image-20210313140349218](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210313140349218.png)

DOM 事件流

![image-20210313154311764](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210313154311764.png)

![image-20210313154414223](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210313154414223.png)

事件发生时会在元素节点之间按照特定的顺序传播，这个传播过程即DOM事件流。
注意
1. Js代码中只能执行捕获或者冒泡其中的一个阶段。
2. onclick 和attachEvent只能得到冒泡阶段。
3. addEventListener(type，listener[,useCapture])第三个参数如果是true，表示在事件捕
  获阶段调用事件处理程序;如果是false (不写默认就是false )，表示在事件冒泡阶段调用事件处理程序。
4. **实际开发中我们很少使用事件捕获，我们更关注事件冒泡。**
5. **有些事件是没有冒泡的，比如onblur、onfocus、onmouseenter、onmouseleave**
6. **事件冒泡有时候会带来麻烦，有时候又会帮助很巧妙的做某些事件，我们后面讲解。**

**事件对象**

![image-20210313161309530](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210313161309530.png)

4．这个事件对象我们可以自己命名比如event . evt、e

5．事件对象也有兼容性问题ie678通过 window.event

![image-20210313161829916](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210313161829916.png)

这个event是个形参，系统帮我们设定为事件对象，不需要传递实参过去。
当我们注册事件时，event对象就会被系统自动创建，并依次传递给事件监听器（事件处理函数)。

![image-20210313161856292](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210313161856292.png)

注意：

  e.target返回的是触发事件的对象（元素)
  this 返回的是绑定事件的对象（元素)   

也就是说： 假如是点击事件，target 返回的是你点击的那个对象，而绑定的对象可能只是点击对象的父盒子，父盒子将点击的对象包含在内，所以两者是有区别的

![image-20210313162807838](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210313162807838.png)

![image-20210313162858024](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210313162858024.png)

![image-20210313163559497](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210313163559497.png)

阻止事件冒泡

![image-20210313164141693](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210313164141693.png)

![image-20210313164156754](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210313164156754.png)

**事件委托**
事件委托也称为事件代理，在jQuery里面称为事件委派。**事件委托的原理**
不是每个子节点单独设置事件监听器，而是事件监听器设置在其父节点上，然后利用冒泡原理影响设置每个子节点。以上案例:给ul注册点击事件，然后利用事件对象的target来找到当前点击的li，,因为点击li，事件会冒泡到ul上，u有注册事件，就会触发事件监听器。
**事件委托的作用**
我们只操作了一次DOM，提高了程序的性能。

![image-20210313164734701](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210313164734701.png)

![image-20210313170739431](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210313170739431.png)

client鼠标在可视区的x和y坐标 不管滚动条有没有滚动都是计算在可视区的坐标

page 则是在文档页面中的坐标

鼠标移动事件:mousemove

图片跟随鼠标移动 案例

![image-20210313172331325](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210313172331325.png)

键盘事件

![image-20210313172724648](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210313172724648.png)

键盘事件对象

![image-20210313173929648](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210313173929648.png)

### 操作元素

innerText

innerHTML 

![image-20210313133555103](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210313133555103.png)



以前的做法:动态创建元素createElement，但是元素里面内容较多，需要innerHTML赋值在appendChild追加到父元素里面.
现在高级做法:利用 **insertAdjacentHTML()** 可以直接把字符串格式元素添加到父元素中

appendChild 不支持追加字符串的子元素, insertAdjacentHTML 支持追加字符串的元素

具体查文档



remove() 方法可以直接删除指定的元素



getAttribute

![image-20210312133720797](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210312133720797.png)

![image-20210312134047875](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210312134047875.png)

![image-20210312134139184](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210312134139184.png)

![image-20210311202824635](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311202824635.png)

![image-20210311203314451](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311203314451.png)

**元素属性的操作**

![image-20210311204652379](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311204652379.png)

**表单元素的属性操作**
利用DOM可以操作如下表单元素的属性∶
type、 value、checked、 selected、disabled

![image-20210311213241515](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311213241515.png)

**样式属性操作**
我们可以通过JS修改元素的大小、颜色、位置等样式。

1. element.style
  行内样式操作

  ![image-20210311220658094](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311220658094.png)

  其中 Js修改style样式操作，产生的是行内样式，**css权重比较高**

2. element.className类名样式操作

   ![image-20210311223746567](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311223746567.png)
   
   ![image-20210311224233317](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311224233317.png)

![image-20210311224346473](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311224346473.png)

#### 循环精灵图

![image-20210311224736722](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210311224736722.png)

#### 反复两个效果

可以通过设置一个 flag = 0 , 当等于 0 是其中一个效果，等于 1 是另外一种效果，然后通过判断 flag 的值来显示不同的效果，同时改变flag的值。

#### 操作元素总结

![image-20210312094626974](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210312094626974.png)

#### 排他思想

![image-20210312114749895](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210312114749895.png)

#### 自定义属性

![image-20210312210256463](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210312210256463.png)

![image-20210312210727828](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210312210727828.png)

### 节点操作

![image-20210312211400223](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210312211400223.png)

![image-20210312211455593](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210312211455593.png)

![image-20210312211840432](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210312211840432.png)

#### 查找结点

父级节点  **parentNode**

![image-20210312212144461](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210312212144461.png)

childrenNodes

![image-20210312212653874](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210312212653874.png)

**children**

![image-20210312212759552](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210312212759552.png)

firstChild    lastChild

![image-20210312213659082](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210312213659082.png)

firstElementChild    lastElementChild

![image-20210312213810834](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210312213810834.png)

![image-20210312214100030](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210312214100030.png)

![image-20210312214009059](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210312214009059.png)

兄弟节点  （实际开发中， 使用比较少）

因为会包括文本节点 **不推荐使用**

1. node.nextSibling
  nextsibling 返回当前元素的下一个兄弟节点，找不到则返回null。同样，也是包含所有的节点。

2. node.previousSibling

  **推荐使用** 下面的方式

3. node .nextElementsibling
  nextElementsibling返回当前元素下一个兄弟元素节点，找不到则返回null。

4. node .previousElementsibling

   **注意∶这两个方法有兼容性问题，IE9以上才支持。**

![image-20210312221130808](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210312221130808.png)



我们想要页面添加一个新的元素: 1. 创建元素2．添加元素

#### 创建节点

document.createElement ( 'tagName ' )
    document.createElement()方法创建由tagName 指定的HTML元素。因为这些元素原先不存在，是根据我们的需求动态生成的，所以我们也称为动态创建元素节点。

#### 添加节点

1. node.appendchild (child)
node.appendChild()方法将一个节点添加倒到指定父节点的子节点**列表末尾**。类似于css里面的after伪元素。

2. node.insertBefore (child，指定元素)
node.insertBefore()方法将一个节点添加到父节点的指定子节点前面。类似于css里面的before伪元素。

#### 删除节点

node. removeChild ( child)
node.removechild ()方法从DOM中删除一个子节点，返回删除的节点。

#### 复制节点(克隆节点)

node.cloneNode ( )
node.cloneNode()方法返回调用该方法的节点的一个副本。也称为克隆节点/拷贝节点
注意∶

1. 如果括号参数为空或者为false，则是浅拷贝，即只克隆复制节点本身，不克隆里面的子节点。
2. 如果括号参数为true，则是深度拷贝，会复制节点本身以及里面所有的子节点。

####三种创建元素的方法区别

![image-20210313124538190](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210313124538190.png)

### DOM 核心总结

建增删改查 属性操作 事件操作

+ 创建
  1. document.write
  2. innerHTML
  3. createElement

+ 增
  1.appendChild
  2.insertBefore

+ 删
  1.removeChild

+ 改
  主要修改dom的元素属性，dom元素的内容、属性,表单的值等
  1．修改元素属性: src、href、title等
  2．修改普通元素内容:innerHTML、innerText
  3.修改表单元素: value、type、disabled等
  4.修改元素样式: style、className

+ 查
  主要获取查询dom的元素

  1. DOM提供的API方法: getElementByld、getElementsByTagName 古老用法不太推荐
  2. H5提供的新方法: querySelector、querySelectorAll提倡
  3. 利用节点操作获取元素∶父(parentNode)、子(children)、兄(previousElementSibling.
    nextElementSibling)提倡

+ 属性操作
  主要针对于自定义属性。
  1.setAttribute:设置dom的属性值

  2.getAttribute:得到dom的属性值

  3.removeAttribute移除属性

+ ![image-20210313131602950](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210313131602950.png)

## BOM

![image-20210314104106400](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314104106400.png)

![image-20210314104244786](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314104244786.png)

 ![image-20210314104900343](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314104900343.png)

### window 常见事件

+ 窗口加载事件

onload

![image-20210314105208572](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314105208572.png)

如果要写多个 onload 事件 用addEventListener

DOMContentLoaded

![image-20210314105421163](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314105421163.png)

load 等页面内容全部加载完毕，包含页面dom元素图片 flash css 等等
DONContentLoaded 是DOM加载完毕，不包含图片 falsh css等就可以执行加载速度比load更快一些

+ 调整窗口大小事件

  onresize innerWidth

![image-20210314110046890](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314110046890.png)

+ 两种定时器

  1. setTimeOut

  ![image-20210314110956781](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314110956781.png)

  回调函数

  ![image-20210314111057123](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314111057123.png)

clearTimeOut

停止定时器

![image-20210314112236318](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314112236318.png)

2. setInterval

![image-20210314112606558](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314112606558.png)

setTimeout 延时时间到了，就去调用这个回调函数，只调用一次就结束了这个定时器
setInterval 每隔这个延时时间，就去调用这个回调函数，会调用很多次，重复调用这个函数

clearInterval

### location

![image-20210314151033861](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314151033861.png)

+ URL

![image-20210314151120481](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314151120481.png)

![image-20210314151312786](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314151312786.png)

**重点记住: href 和 search**

location 对象的方法  assign replace  reload

![image-20210314161419882](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314161419882.png)

+new

JavaScript中可以在某个元素前使用 ‘+’ 号，这个操作是将该元素转换成Number类型，如果转换失败，那么将得到 NaN。

### navigation 对象

![image-20210314161818163](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314161818163.png)

### history

![image-20210314162219347](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314162219347.png)

# js 是单线程

JS是单线程
JavaScript语言的一大特点就是单线程，也就是说，同一个时间只能做一件事。这是因为JavaScript这门脚本语言诞生的使命所致——JavaScript是为处理页面中用户的交互，以及操作DOM而诞生的比如我们对某个DOM元素进行添加和删除操作，不能同时进行。应该先进行添加，之后再删除。

单线程就意味着，所有任务需要排队，前一个任务结束，才会执行后一个任务。这样所导致的问题是∶如果JS执行的时间过长，这样就会造成页面的渲染不连贯，导致页面渲染加载阻塞的感觉。

## 同步和异步

为了解决这个问题，利用多核CPU的计算能力，HTMLS提出Web Worker标准，允许JavaScript脚本创建多个线程。于是，JS中出现了同步和异步。
**同步**
前一个任务结束后再执行后一个任务，程序的执行顺序与任务的排列顺序是一致的、同步的。比如做饭的同步做法:我们要烧水煮饭,等水开了(10分钟之后)，再去切菜，炒菜。
**异步**
你在做一件事情时，因为这件事情会花费很长时间，在做这件事的同时，你还可以去处理其他事情。比如做饭的异步做法，我们在烧水的同时，利用这10分钟，去切菜，炒菜。

**他们的本质区别:这条流水线上各个流程的执行顺序不同。**

![image-20210314150128910](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314150128910.png)

![image-20210314150228463](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314150228463.png)

![image-20210314150843722](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314150843722.png)

# this 的指向问题

![image-20210314145107573](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314145107573.png)

![image-20210314145132068](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314145132068.png)

![image-20210314145203026](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314145203026.png)

# 倒计时代码

```javascript
function countDown(time) {
            var nowTime = +new Date(); //返回的是当前时间总的毫秒数
            var inputTime = +new Date(time); //返回的是用户输入时间总的毫秒数
            var times = (inputTime - nowTime) / 1000; // times是剩余时间总的秒数
            var d = parseInt(times / 60 / 60 / 24); //天
            d = d < 10 ? '0' + d : d;
            var h = parseInt(times / 60 / 60 % 24); //时
            h = h < 10 ? '0' + h : h;
            var m = parseInt(times / 60 % 60); //分
            m = m < 10 ? '0' + m : m;
            var s = parseInt(times % 60); //当前的秒
            s = s < 10 ? '0' + s : s;
            return d + '天' + h + '时' + m + '分' + s + '秒';
        }
```

# 计算鼠标在盒子中的坐标

![image-20210314164746523](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314164746523.png)

应用: 鼠标拖拽盒子移动

```javascript
title.addEventListener('mousedown', function(e) {
            var x = e.pageX - login.offsetLeft; // 获得鼠标在盒子中的坐标
            var y = e.pageY - login.offsetTop;
            document.addEventListener('mousemove', move)

            function move(e) {
                login.style.left = e.pageX - x + 'px';
                login.style.top = e.pageY - y + 'px';
            }
            document.addEventListener('mouseup', function() {
                document.removeEventListener('mousemove', move)

            })
        })
```



# pc 端网页特效

## offset

![image-20210314163159181](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314163159181.png)

![image-20210314163922725](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314163922725.png)

offsetTop offsetLeft:  如果没有父亲 或者父亲没有定位，则以body为准

**offset style区别**

![image-20210314164309649](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314164309649.png)

client

![image-20210314173136559](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314173136559.png)

**立即执行函数**

不需要调用，立马执行

( function(){} ) ()   或  ( function(){} () )
主要作用︰创建一个独立的作用域。避免了命名冲突问题

scroll

![image-20210314175948247](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314175948247.png)

![image-20210314180337492](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314180337492.png)

他们主要用法︰

1. offset系列经常用于获得元素位置offsetLeft offsetTop
2. client经常用于获取元素大小clientWidth clientHeight
3. scroll经常用于获取滚动距离scrollTop scrollLeft
4. 注意页面滚动的距离通过**window.pageYOffset**获得  没有单位
5. 滚动窗口至文档中的特定位置。window.scroll(x, y)        x , y 没有单位

**mouseenter mouseover的区别**
mouseenter鼠标事件

+ 当鼠标移动到元素上时就会触发mouseenter事件
+ 类似mouseover，它们两者之间的差别是
+ mouseover鼠标经过自身盒子会触发，经过子盒子还会触发。mouseenter只会经过自身盒子触发
+ 之所以这样，就是因为mouseenter不会冒泡
+ 跟mouseenter搭配鼠标离开mouseleave同样不会冒泡

## 节流阀

防止轮播图按钮连续点击造成播放过快。
节流阀目的:当上一个函数动画内容执行完毕，再去执行下一个函数动画，让事件无法连续触发。
核心实现思路︰利用回调函数，添加一个变量来控制，锁住函数和解锁函数。

# canvas

![image-20210314201126528](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210314201126528.png)

# 动画函数

核心原理∶通过定时器setInterval()不断移动盒子位置。
实现步骤∶

1. 获得盒子当前位置
2. 让盒子在当前位置加上1个移动距离
3. 利用定时器不断重复这个操作
4. 加一个结束定时器的条件
5. 注意此元素需要添加定位，才能使用element.style.left

用下面函数的**前提**是需要移动的元素开启了定位，因为代码中需要修改盒子的 style.left 值

```javascript
function animate(obj, target, callback) {
    // console.log(callback);  callback = function() {}  调用的时候 callback()

    // 先清除以前的定时器，只保留当前的一个定时器执行
    clearInterval(obj.timer);
    obj.timer = setInterval(function() {
        // 步长值写到定时器的里面
        // 把我们步长值改为整数 不要出现小数的问题
        // var step = Math.ceil((target - obj.offsetLeft) / 10);
        var step = (target - obj.offsetLeft) / 10;
        step = step > 0 ? Math.ceil(step) : Math.floor(step);
        if (obj.offsetLeft == target) {
            // 停止动画 本质是停止定时器
            clearInterval(obj.timer);
            // 回调函数写到定时器结束里面
            // if (callback) {
            //     // 调用函数
            //     callback();
            // }
            callback && callback();
        }
        // 把每次加1 这个步长值改为一个慢慢变小的值  步长公式：(目标值 - 现在的位置) / 10
        obj.style.left = obj.offsetLeft + step + 'px';

    }, 15);
}
```

**缓动效果原理**
缓动动画就是让元素运动速度有所变化，最常见的是让**速度慢慢停下来**
思路∶

1. 让盒子每次移动的距离慢慢变小，速度就会慢慢落下来。

2. 核心算法︰(目标值-现在的位置)/ 10做为每次移动的距离步长

3. 停止的条件是:让当前盒子位置等于目标位置就停止定时器
4. 步长值需要取整（ 用 Math.ceil() ），因为不去整的话会有小数，这样的话可能会累计误差，导致不能完全到达停止位置

![image-20210316215723229](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210316215723229.png)

# 移动端

## 事件

touchstart      touchmove    touchend

![image-20210318134259525](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210318134259525.png)

### 事件对象

![image-20210318140246647](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210318140246647.png)

![image-20210318141022186](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210318141022186.png)

![image-20210318141040880](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210318141040880.png)

 阻止默认的屏幕滚动  e.preventDefault();

+ 因为移动端不用考虑兼容性，可以直接使用 css3 ，所以可以利用过渡来形成动画效果

  transition

  ==在经常和 :hover 一起 搭配使用==

  ![image-20201212131302523](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20201212131302523.png)

  如果想要写多个属性，利用逗号进行分割 或者 属性写 all 就可以了

  js 检测过渡完成事件 transitionend

  

+  classList属性是HTML5新增的一个属性，返回元素的类名。但是ie10以上版本支持。

![image-20210318162137059](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210318162137059.png)

![image-20210318162431946](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210318162431946.png)

![image-20210318162326356](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210318162326356.png)

## **click延时**解决方案

移动端click事件会有300ms的延时，原因是移动端屏幕双击会缩放(double tap to zoom)页面。

![image-20210318200458923](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210318200458923.png)

![image-20210318200552772](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210318200552772.png)

上面这种方法，如果有多个事件都需要解决延时，就需要每个事件都绑定，比较麻烦

+ 解决方案三（最常用）

 ![image-20210318203524159](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210318203524159.png)

在官网的 lib 文件下

本地已下载在            `D:\学习文件\笔记OLY\JavaScript_new\fastclick.js`

使用方法：

1. 首先在 HTML 文件中引用 fastclick.js
2. 然后再自己写的 js 文件中引入

```javascript
<script>
        if ('addEventListener' in document) {
            document.addEventListener('DOMContentLoaded', function() {
                FastClick.attach(document.body);
            }, false);
        }  
</script>
```

完成后就能够把所有的延时都取消

## Swiper 插件（轮播图）

3.3 Swiper插件的使用
中文官网地址: https://www.swiper.com.cn/

1. 引入插件相关文件。
2. 按照规定语法使用（将源码依次引入，注意不要更改里面的结构和类名）

​        首先再官网找到想要的样式，然后根据编号再下好的文件中的demo文件夹中根据编号找到，然后打开查看源码，根据源码中的需要引入相关文件，记住自己的 js 文件要在文档的 js 文件的引入下面，因为我们自己写的 js 文件是依赖于文档文件的。

其他移动端常见插件
superslide : http://www.superslide2.com/

iscroll : https://github.com/cubiq/iscroll

**插件的使用总结**

1. 确认插件实现的功能

2. 去官网查看使用说明

3. 下载插件
4. 打开demo实例文件，查看需要引入的相关文件，并且引入
5. 复制demo实例文件中的结构html，样式css以及js代码

**zy.media.js  插件**

![image-20210318212218730](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210318212218730.png)

# 框架

![image-20210318212756397](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210318212756397.png)

![image-20210318213620174](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210318213620174.png)

# 本地存储

![image-20210318214305468](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210318214305468.png)

## window.sessionStorage

window 可省略

1、生命周期为关闭浏览器窗口

2、在同一个窗口(页面)下数据可以共享

3、以键值对的形式存储使用

![image-20210318222139478](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210318222139478.png)

```javascript
<body>
    <input type="text">
    <button class="set">存储数据</button>
    <button class="get">获取数据</button>
    <button class="remove">删除数据</button>
    <button class="del">清空所有数据</button>
    <script>
        console.log(localStorage.getItem('username'));

        var ipt = document.querySelector('input');
        var set = document.querySelector('.set');
        var get = document.querySelector('.get');
        var remove = document.querySelector('.remove');
        var del = document.querySelector('.del');
        set.addEventListener('click', function() {
            // 当我们点击了之后，就可以把表单里面的值存储起来
            var val = ipt.value;
            sessionStorage.setItem('uname', val);
            sessionStorage.setItem('pwd', val);
        });
        get.addEventListener('click', function() {
            // 当我们点击了之后，就可以把表单里面的值获取过来
            console.log(sessionStorage.getItem('uname'));

        });
        remove.addEventListener('click', function() {
            // 
            sessionStorage.removeItem('uname');

        });
        del.addEventListener('click', function() {
            // 当我们点击了之后，清除所有的
            sessionStorage.clear();

        });
    </script>
</body>
```

## localStorage

![image-20210318222940642](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210318222940642.png)

```javascript
<body>
    <input type="text">
    <button class="set">存储数据</button>
    <button class="get">获取数据</button>
    <button class="remove">删除数据</button>
    <button class="del">清空所有数据</button>
    <script>
        var ipt = document.querySelector('input');
        var set = document.querySelector('.set');
        var get = document.querySelector('.get');
        var remove = document.querySelector('.remove');
        var del = document.querySelector('.del');
        set.addEventListener('click', function() {
            var val = ipt.value;
            localStorage.setItem('username', val);
        })
        get.addEventListener('click', function() {
            console.log(localStorage.getItem('username'));

        })
        remove.addEventListener('click', function() {
            localStorage.removeItem('username');

        })
        del.addEventListener('click', function() {
            localStorage.clear();

        })
    </script>
</body>
```

JSON.stringify()

![image-20210326141215177](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210326141215177.png)

注意点1∶本地存储 localStorage 里面只能存储字符串格式，因此需要把对象转换为字符串 **JSON.stringify(data)** 。

注意点2∶获取本地存储数据，需要把里面的字符串转换为对象格式 **JSON.parse()** 我们才能使用里面的数据。

# jQuery

中文文档： https://jquery.cuishifeng.cn/

## 引入方法

1. 下载至本地库
2. CDN 远程库   www.bootcdn.cn   直接复制路径就行，以减轻服务器压力

![image-20210324144301442](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210324144301442.png)

![image-20210324144424529](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210324144424529.png)

js 库
官网地址: https://jquery.com/

下载好后在网页中把代码复制过来 

![image-20210319092244095](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210319092244095.png)

入口函数

![image-20210319093424721](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210319093424721.png)

1. 使用jQuery**核心函数**:   $/jQuery
2. 使用jQuery**核心对象**:   执行$()返回的对象

![image-20210324141419607](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210324141419607.png)

![image-20210319143720392](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210319143720392.png)

![image-20210324153748410](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210324153748410.png)

## **DOM 对象 和 jQuery 对象 转换**

![image-20210319174651177](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210319174651177.png)

![image-20210324154325319](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210324154325319.png)

## 选择器

![image-20210319184206741](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210319184206741.png)

 ![image-20210319184410762](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210319184410762.png)

+ 隐式迭代

jQuery设置样式方法：    $('div').css('属性', '值')

![image-20210319184716684](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210319184716684.png)

+ 筛选选择器

![image-20210319184848655](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210319184848655.png)

+ 筛选方法 （记得加括号）

![image-20210324163644933](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210324163644933.png)

parent() 返回的是最近一级的父级 

parents(‘选择器’) 可以返回指定祖先元素，这样就不用一层一层的找了

eq()   是指第几个元素



toFixed(2)  //保留两位小数

## 排他思想

想要多选一的效果，排他思想:当前元素设置样式，其余的兄弟元素清除样式.

应用隐式迭代

![image-20210324164123449](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210324164123449.png)

jQuery得到当前元素索引号   $(this).index()

show()  //显示元素

hide()   //隐藏元素

## 样式操作

操作 css 方法

![image-20210324165253645](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210324165253645.png)

![image-20210324165333914](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210324165333914.png)

设置类样式方法

addClass()   removeClass()   toggleClass()

![image-20210324165841656](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210324165841656.png)

**类操作与className区别**

原生 JS 中 className 会覆盖元素原先里面的类名。
jQuery里面类操作只是对指定类进行操作，不影响原先的类名。

链式编程操作

![image-20210324170711098](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210324170711098.png)

## 动画效果

![image-20210324171442904](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210324171442904.png)

具体的也可以自己去查阅 jQuery 的 API 的文档

+ show()

![image-20210324171555135](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210324171555135.png)

slideDown()  slideUp()  slideToggle()   参数所代表的含义都一样

![image-20210324173947795](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210324173947795.png)

fadeIn()   fadeOut()  fadeToggle()   参数做代表的含义都一样

![image-20210324180153182](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210324180153182.png)

fadeTo()   修改透明度![image-20210324180356683](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210324180356683.png)

**自定义动画 animate**

![image-20210324214859854](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210324214859854.png)

![image-20210324215232940](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210324215232940.png)



**事件切换  hover()**

事件切换 hover就是鼠标经过和离开的复合写法

![image-20210324175046540](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210324175046540.png)

(3)事件切换hover如果只写一个函数，那么鼠标经过和鼠标离开都会触发这个函数



**动画队列及其停止排队方法**

1.动画或效果队列

动画或者效果一旦触发就会执行，如果多次触发，就造成多个动画或者效果排队执行。

2.停止排队
stop()
(1 ) stop()方法用于停止动画或效果。

(2)注意:stop()写到动画或者效果的==前面，相当于停止结束上一次的动画==。 

eg:  $(this).stop().slideUp(200)

## 属性操作

设置或获取元素固有属性值  prop()

![image-20210325141056029](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210325141056029.png)

设置或获取元素自定义属性 attr()

![image-20210325141636775](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210325141636775.png)

**H5 自定义数据属性**: HTML5规定可以为元素添加非标准的属性，但要添加前缀data-, 目的是为元素提供与渲染无关的信息，或者提供语义信息。

```html
 <div id="myDiv" data-appId="12345" data-myname="Nicholas"></div>  
```

添加自定义属性之后，可以通过元素的dataset属性来访问自定义属性的值。

数据缓存 data()

![image-20210325143118586](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210325143118586.png)

![image-20210325143538549](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210325143538549.png)

:checked  查找被选中的表单元素，返回被选中元素的一个数组，数组里面有 length 属性，也就可以得出被选中元素的个数。

## 内容文本值

html()   text()

![image-20210325150418571](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210325150418571.png)

val()

**表单**的值   

val()          (相当于原生value)

val("内容")   



截取字符串substr(1) //从位置1开始截取（从0 开始）

## 元素操作

遍历、创建、添加、删除

+ 遍历

each()

![image-20210325162707114](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210325162707114.png)

上面的方法适合于遍历 DOM 元素对象

![image-20210325164031952](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210325164031952.png)

适合遍历数组，对象

![image-20210325164115691](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210325164115691.png)

+ 创建

![image-20210325184227166](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210325184227166.png)

+ 添加

内部添加 append()  prepend()

![image-20210325184415721](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210325184415721.png)

![image-20210325184428502](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210325184428502.png)

外部添加   after()  before()

![image-20210325184612235](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210325184612235.png)

+ 删除   remove()  empty()   html("")   （ html() 是用来得到标签里面的内容的，括号内换成空字符串也就相当于是清空 ）

![image-20210325184956746](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210325184956746.png)

## 事件

###事件注册

与原生 js 类似

![image-20210325195700652](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210325195700652.png)

###事件处理

on()

![image-20210325195842590](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210325195842590.png)

优势

![image-20210325200315042](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210325200315042.png)

on() 方法优势2∶
  可以**事件委派**（事件委托）操作。事件委派的定义就是，把原来加给子元素身上的事件绑定在父元素身上，就是把事件委派给父元素。可以理解成事件冒泡

![image-20210325202611846](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210325202611846.png)

on()方法优势3∶
动态创建的元素，click() 没有办法绑定事件，==on() 可以给后面动态生成的元素绑定事件==

![image-20210325203042122](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210325203042122.png)





off() **解绑事件**

off() 方法可以移除通过on()方法添加的事件处理程序。

![image-20210325212136613](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210325212136613.png)

one()  只触发依次，参数格式和 on() 类似



自动触发事件 trigger()

有些事件希望自动触发,比如轮播图自动播放功能跟点击右侧按钮一致。可以利用定时器目动段发右侧按钮点击事件，不必鼠标点击触发。

```javascript
element.click() //第一种简写形式  会触发元素的默认行为
element.trigger("type") //第二种自动触发模式  会触发元素的默认行为

 $("p").on("click", function () {
                alert("hi~");
            });
            $("p").trigger("click"); //此时自动触发点击事件，不需要鼠标点击

element.triggerHandler("type") //第三种自动触发模式  不会触发元素的默认行为，比如说input元素 自动触发 focus 时不会有光标出现。


```

###事件对象

事件被触发，就会有事件对象的产生。

element.on (events, [selector] , function (**event**) {})    事件对象跟原生 js 有着类似的方法，可参考原生 js 

阻止默认行为: event.preventDefault() 或者 return false

阻止冒泡: event.stopPropagation()

## 其他方法

### 拷贝对象

$.extend() 方法

![image-20210325223623469](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210325223623469.png)

![image-20210325223107997](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210325223107997.png)

1. 浅拷贝把原来对象里面的复杂类型地址拷贝给目标对象，会覆盖复杂数据类型里面原来的数据
2. 深拷贝把里面的数据完全复制一份给目标对象，如果里面有不冲突的属性，会合并到一起

### 多库共存

![image-20210325224432647](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210325224432647.png)

### jQuery插件

jQuery功能比较有限，想要更复杂的特效效果，可以借助于jQuery插件完成。

注意: 这些插件也是依赖于jQuery来完成的，所以必须要先引入jQuery文件，因此也称为jQuery插件。

**jQuery插件常用的网站:**

1. jQuery插件库   http://www.jq22.com/

2. jQuery之家  http://www.htmleaf.com/   推荐 因为是免费滴

   下载插件后看里面的demo，然后查看源代码，仿照里面进行的链接进行引入和复制粘贴

**jQuery插件使用步骤:**

1. 引入相关文件。（jQuery文件 和 插件文件)
2. 复制相关html、css、js (调用插件)

jQuery插件演示:

1. 瀑布流
2. 图片懒加载(图片使用延迟加载在可提高网页下载速度。它也能帮助减轻服务器负载)

当我们页面滑动到可视区域，再显示图片。

我们使用jquery插件库 EasyLazyload。注意，此时的js引入文件和js调用必须写到DOM元素(图片）最后面      **使用有点问题**

3. 全屏滚动( fullpage.js )
   gitHub : https://github.com/alvarotrigo/fullPage.js
   中文翻译网站:http://www.dowebok.com/demo/2014/77/

### 尺寸和位置操作

width()  height()  innerWidth()  innerHight()  outerWidth()  outerHeight()  

![image-20210326182133272](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210326182133272.png)**jQuery 位置**

位置主要有三个: offset()   position()  scrollTop() / scrollLeft()

![image-20210326184928387](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210326184928387.png)

![image-20210326185140914](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210326185140914.png)

获取距离**带有定位父级**位置（偏移)  position 如果没有带有定位的父级，则以文档为准，这个方法**只能获取不能设置偏移**

被卷去的头部scrollTop()

被卷去的左侧scrollLeft()

# 面向对象 ES6

+ **面向过程编程**  POP(Process-oriented programming)
      面向过程就是分析出解决问题所需要的步骤，然后用函数把这些步骤一步一步实现，使用的时候再一个一个的依次调用就可以了。

+ **面向对象编程**  OOP(Object Oriented Programming)
      面向对象是把事务分解成为一个个对象，然后由对象之间分工与合作。

![image-20210319190436251](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210319190436251.png)

![image-20210319190616184](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210319190616184.png)

## 对象 和 类

![image-20210319190900077](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210319190900077.png)

![image-20210319190940060](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210319190940060.png)

![image-20210319191012087](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210319191012087.png)

+ 创建类  

![image-20210319191054091](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210319191054091.png)

类         **constructor  构造函数**
constructor()方法是类的构造函数(默认方法)，**用于传递参数，返回实例对象**，通过new命令生成对象实例时，自动调用该方法。如果没有显示定义,类内部会自动给我们创建一个constructor()

![image-20210319191510847](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210319191510847.png)

![image-20210319191700324](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210319191700324.png)

+ 类 **添加方法**    

1. 不需要加 function 关键字
2. 多个函数之间不需要 添加逗号进行分割

![image-20210319191755027](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210319191755027.png)

## 继承

![image-20210319192522694](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210319192522694.png)

**super 关键字**    可以实现子类向父类传递参数

用于访问和调用对象父类上的函数。可以调用父类的构造函数，也可以调用父类的普通函数

 调用构造函数如下

![image-20210319192750112](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210319192750112.png)

调用普通函数如下

![image-20210319193351410](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210319193351410.png)



==三个注意点:==
1．在ES6中类没有变量提升，所以必须先定义类，才能通过类实例化对象.

![image-20210319195636799](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210319195636799.png)

也就是 super 要写在 this 的前面

2．类里面的共有属性和方法一定要加this使用.

![image-20210319200252898](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210319200252898.png)

3．类里面的this指向问题.

constructor里面的 this 指向的是创建的实例对象

方法中的 this 指向的是调用这个方法的对象，也就是调用

# 构造函数和原型 ES6 前

es6 之前是通过构造函数和原型 实现的类的

**概述**
在典型的OOP的语言中(如Java )，都存在类的概念，类就是对象的模板，对象就是类的实例，但在ES6之前，JS中并没用引入类的概念

ES6，全称ECMAScript 6.0，2015.06发版。但是目前浏览器的JavaScript是ES5版本，大多数高版本的浏览器也支持ES6，不过只实现了ES6的部分特性和功能。

在ES6之前，对象不是基于类创建的，而是用一种称为**构建函数**的特殊函数来定义对象和它们的特征。

创建对象可以通过以下三种方式:

1.对象字面量

2.new Object()

3.自定义构造函数

![image-20210320092836619](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320092836619.png)

![image-20210320093045652](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320093045652.png)

## 实例成员 静态成员

![image-20210320093435995](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320093435995.png)

![image-20210320093554890](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320093554890.png)

 解决方法

构造函数原型 **prototype**  也称为**原型对象**

构造函数通过原型分配的函数是所有对象所共享的。

JavaScript规定，每一个构造函数都有一个prototype属性，指向另一个对象。注意这个prototype就是一个对象，这个对象的所有属性和方法，都会被构造函数所拥有。

我们可以把那些不变的方法，直接定义在prototype对象上，这样所有对象的实例就可以**共享**这些方法。

```javascript
Star.protype.sing = function() {
  console.log('我会唱歌')；
}
```

==一般情况下,我们的公共属性定义到构造函数里面，公共的方法我们放到原型对象身上==

对象原型 \__proto__

![image-20210320101057341](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320101057341.png)

constructor 构造函数  

![image-20210320132433546](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320132433546.png)

![image-20210320132511714](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320132511714.png)

![image-20210320133113397](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320133113397.png)

## 原型链

![image-20210320133710304](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320133710304.png)

![image-20210320134200705](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320134200705.png)

## this 指向问题

![image-20210320134627616](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320134627616.png)

![image-20210320140327153](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320140327153.png)

## 继承

ES6之前并没有给我们提供extends继承。我们可以通过**构造函数+原型对象**模拟实现继承，被称为**组合继承**

call()

![image-20210320140923531](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320140923531.png)

+ 借用构造函数继承父类型**属性**

![image-20210320143111170](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320143111170.png)

+ 借用构造函数继承父类型**方法**

![image-20210320144417702](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320144417702.png)

## ES5 中的新增方法

+ 数组方法
  迭代(遍历)方法: forEach()、map()、filter()、some()、every() ;

forEach()    return 不可以终止循环

![image-20210320145349175](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320145349175.png)

filter()        return 不可以终止循环

![image-20210320145519128](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320145519128.png)

![image-20210320145633297](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320145633297.png)

返回的是元素大于等于20 的新数组

some()          return 可以终止循环

![image-20210320150023110](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320150023110.png)

![image-20210320150204961](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320150204961.png)

![image-20210320150400092](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320150400092.png)

**字符串方法**

trim()

![image-20210320185430598](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320185430598.png)

**对象方法**

keys()         获取对象的所有属性名

![image-20210320185452047](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320185452047.png)

defineProperty()

![image-20210320185824062](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320185824062.png)

![image-20210320190019940](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320190019940.png)

属性有的话是修改，没有的话是添加

![image-20210320190410928](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320190410928.png)

enumerable 默认是不能被枚举，也就是说，只要用了 defineProperty() 这个方法，就算你没有设置enumerable 的属性值，也是默认不能被枚举的，也就是循环的时候该值不会被遍历出来



delete obj.address ;  删除元素



# 严格模式

![image-20210320223321499](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320223321499.png)

## 开启严格模式

![image-20210320223532314](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320223532314.png)

![image-20210320223623108](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320223623108.png)

![image-20210320223714260](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320223714260.png)

##严格模式中的变化

![image-20210320224022066](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320224022066.png)

![image-20210320224949236](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320224949236.png)

![image-20210320225350011](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320225350011.png)

# 高阶函数  

![image-20210320225900517](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320225900517.png)

# 闭包

closure

变量作用域
变量根据作用域的不同分为两种:全局变量和局部变量。

1.函数内部可以使用全局变量。
2.函数外部不可以使用局部变量。
3.当函数执行完毕，本作用域内的局部变量会销毁。

**概念**

![image-20210320230522686](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210320230522686.png)

这个作用域所在的函数就是闭包函数 

闭包的主要作用：延伸了变量的作用范围

```javascript
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>

<body>
    <ul class="nav">
        <li>榴莲</li>
        <li>臭豆腐</li>
        <li>鲱鱼罐头</li>
        <li>大猪蹄子</li>
    </ul>
    <script>
        // 闭包应用-点击 li 输出当前 li 的索引号
        // 1. 我们可以利用动态添加属性的方式
        var lis = document.querySelector('.nav').querySelectorAll('li');
        for (var i = 0; i < lis.length; i++) {
            lis[i].index = i;
            lis[i].onclick = function () {
                console.log(this.index);
            }
        }
        // 2. 利用闭包的方式得到当前 li 的索引号
        for (var i = 0; i < lis.length; i++) {
            //利用for循环创建了4个立即执行函数
            (function (i) {
                lis[i].onclick = function () {
                    console.log(i);
                }
            })(i);
        }
    </script>
</body>

</html>
```

另一个案例

```javascript
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>

<body>
    <script>
        //打车起步价13(3公里内)，之后每多一公里增加5块钱．用户输入公里数就可以///如果有拥堵情况,总价格多收取10块钱拥堵费
        // function fn() {};
        // fn();
        var car = (function () {
            var start = 13;//起步价 局部变量
            var total = 0; //总价  局部变量
            return {
                //正常的总价
                price: function (n) {
                    if (n <= 3) {
                        total = start;
                    } else {
                        ltotal = start + (n - 3) * 5
                    }
                    return total;
                },
                //拥堵之后的费用
                yd: function (flag) {
                    return flag ? total + 10 : total;
                }
            }
        })();
        console.log(car.price(5));  // 23
        console.log(car.yd(true));  // 33
        console.log(car.price(1));  // 13
        console.log(car.yd(false)); // 13
    </script>
</body>

</html>
```

# 递归

![image-20210321191359687](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321191359687.png)

![image-20210321191659261](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321191659261.png)

![image-20210321192050449](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321192050449.png)

![image-20210321192634500](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321192634500.png)

![image-20210321192658160](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321192658160.png)

上面的改进：让结果返回而不是打印

![image-20210321193333628](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321193333628.png)

## 浅拷贝 深拷贝

1．浅拷贝只是拷贝一层,更深层次对象级别的只拷贝引用.

浅拷贝遇到更深层次的对象是只是拷贝地址，所以拷贝后两者地址指向的是同一个

![image-20210321194407071](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321194407071.png)

![image-20210321194427900](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321194427900.png)

Object.assign( target, ...sources)       es6新增方法可以浅拷贝

例如上面的例子可以这样实现浅拷贝： Object.assign(o, obj);

![image-20210321195902899](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321195902899.png)

2．深拷贝拷贝多层,每一级别的数据都会拷贝.

![image-20210321200746066](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321200746066.png)

![image-20210321200812503](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321200812503.png)

![image-20210321200836803](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321200836803.png)

上面函数中判断类型里边，必须要先判断数组在判断对象，因为数组也属于对象

# 正则表达式

![image-20210321210800483](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321210800483.png)

![image-20210321210932359](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321210932359.png)

+ 创建

![image-20210321211600388](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321211600388.png)

![image-20210321212337847](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321212337847.png)

+ 检测正则表达式 test

![image-20210321211813015](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321211813015.png)

![image-20210321211829552](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321211829552.png)

## 特殊字符（元字符）

![image-20210321211950370](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321211950370.png)

MDN : https://developer.mozila.org/zh-CN/docs/Web/JavaScript/Guide/Regular_Expressions

正则测试工具:http://tool.oschina.net/regex

边界符  ^  $

![image-20210321212305503](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321212305503.png)

![image-20210321212647620](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321212647620.png)

字符类  []

![image-20210321213840801](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321213840801.png)

[-]方括号内部范围符

![image-20210321214017284](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321214017284.png)

字符组合

![image-20210321215021545](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321215021545.png)

![image-20210321214817147](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321214817147.png)

取反符

![image-20210321215048433](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321215048433.png)

![image-20210321214913170](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321214913170.png)

量词符  用来设定某个模式出现的次数

![image-20210321215303178](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321215303178.png)

![image-20210321215340009](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321215340009.png)

![image-20210321215611992](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321215611992.png)

量词设定某个模式出现的次数   /$[a-zA-Z0-9-_]{6,16}^/

![image-20210321220025016](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321220025016.png)

==注意量词中间不要有空格==

![image-20210321220451849](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321220451849.png)

**括号总结**

![image-20210321220919731](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321220919731.png)

 在线测试:   https://c.runoob.com/          里面还有许多其他的测试功能



预定义类

![image-20210321221603925](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321221603925.png)

![image-20210321221716689](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210321221716689.png)

## 替换

replace()

![image-20210322103304760](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210322103304760.png)

参数

![image-20210322103355841](D:\学习文件\笔记OLY\JavaScript_new\JavaScript.assets\image-20210322103355841.png)

