 

+ vsc

  ctrl +  放大字体

  ctrl -  缩小

# Web标准

+ ==Web标准==是由W3C组织和其他标准化组织制定的一些列标准的集合
+ 主要包括==结构(html)、表现(css)和行为(Javascript)==三个方面。  

# 开发技巧

+ 导航栏注意点：

实际开发中，我们不会直接用链接a而是用li包含链接(li+a)的做法。

![image-20201207142119052](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201207142119052.png)

+ 因为页面中的图片太多了，最好不要直接去控制图片，而是给每一个图片套一个父盒子，控制盒子是最好的，以免出现一些不必要的问题。




# 基本骨架

```html
<html>
    <head>
        <title>第一个页面</title>
    </head>
    <body>
        键盘敲烂，工资过万
    </body>
</html>
```

```html
<!DOCTYPE html>
<html lang="en">  
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>
  <h1></h1>
</body>
</html>
```

+ `<!DOCTYPE html>`表示当前页面采用HTML5版本来显示页面

  `<!DOCTYPE>`不是HTML标签，它就是文档类型声明标签。

+ `lang="en"`

  language=English（英文网站） "zh-CN"（中文网站）

+ ` <meta charset="UTF-8">`  表示采用UTF-8来保存文字，如果不写会导致乱码。

# html

## 常用标签

+ `<h1> - <h6>`标题标签

  依据重要性递减    ==独占一行==

```html
<h1>
  我是一级标题
</h1>
```

特点：

+ `<p></p>`段落标签 

  1. 段落中自动换行
  2. 段落间会插入间隙

+ `<br />`换行标签（break）

  1. ==单标签==    **习惯在后面插入一个空格加斜杠表示单标签的意思**
  2. 只是重新开始新的一行，跟段落不一样，段落之间会插入一些垂直的距离。

+ 文本格式化标签

  加粗（\<b>也是加粗）  倾斜  删除线  下划线

  ![image-20201124154620264](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201124154620264.png)

+ `<div>`和`<span>`

  没有语义，它们就是一个盒子，用来装内容的，用来布局

  div  division : 分割、分区      span :  n. 跨度，跨距

  1. \<div>==独占一行==
  2. \<span>一行上可以多个

+ 图像标签（单标签)

  因为页面中的图片太多了，最好不要直接去控制图片，而是给每一个图片套一个父盒子，控制盒子是最好的

  ```html
  <img src="图像URL" />
  ```

  src 是必须属性，用于指定图像文件的路径和文件名

  属性：

  ![image-20201124160714893](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201124160714893.png)

+ 超链接标签\<a> (anchor: 锚)

  在网页中各种网页元素，如文本、图像、表格、视频都可以添加超链接。

  ![image-20201124170156258](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201124170156258.png)

  浏览器为 a 链接默认制定了一个样式，蓝色的 有下划线 a{ color: blue; }

  空链接：`<a href="#">首页</a> `

  阻止链接跳转需要添加javascriptvoid(0); 或者javascript:;

  + 链接分类

    1. 外部链接
    2. 内部链接
    3. 空链接
    4. 下载链接
    5. 网页元素链接
    6. **锚点链接**

    <img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201124172812125.png" alt="image-20201124172812125"  /> 

  + 表头单元格式标签

+ 注释标签

  `<!-- 注释语句 -->`    快捷键： Ctrl + /

+ 表格标签

  主要用于显示、展示数据。

  + 基本语法

    \<table> \<tr> \<td>

    <img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201124205959280.png" alt="image-20201124205959280" style="zoom:50%;" />

    单元格里面可以放任何元素，文字链接图片等都可以。

  + 表头单元格式标签`<th> (table head)`

    表头单元格里面的文本内容**加粗居中**显示

    ```html
    <table>
      <tr>
        <th>姓名</th>
        ...
      </tr>
      ...
    </table>
    ```

  + 表格结构标签

    为了更好表示表格的语义，将表格分割成表格头部和表格主体两大部分，这样可以更好的分清表格结构。

    1.  `<thead>`标签 ： 表格的头部区域，其内部必须拥有\<tr>标签。一般是位于第一行。

    2.  `<tbody>`标签 ： 表格的主体区域 ，主要用于存放数据本体。
    3. 以上两个标签都是放在 \<table><\table> 标签中。

  + 表格属性（实际开发中不常用，通过CSS来设置）

    ![image-20201124213031958](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201124213031958.png)

  + 合并单元格

    方式：

      跨行合并： rowspan='合并单元格的个数'

      跨列合并： clospan='合并单元格的个数'

    ![image-20201125000744644](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201125000744644.png)

    目标单元格：（写合并代码）

      跨行：最上侧单元格为目标单元格，写合并代码

      跨列：最左侧单元格为目标单元格，写合并代码

    <img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201125001214374.png" alt="image-20201125001214374" style="zoom:50%;" />

+ 列表标签

  表格是用来显示数据的，而列表就是用来布局的。

  分为无序列表、有序列表和自定义列表。

  + 无序列表（重点）

    去掉 li 前面的 项目符号(小圆点):  list-style: none; 

    ```html
    <ul>
      <li>列表项1</li>
      <li>列表项2</li>
      ...
    </ul>
    ```

    <img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201125004102675.png" alt="image-20201125004102675" style="zoom:50%;" />

  + 有序列表(order list)

    ```html
    <ol>
        <li>列表项1</li>
        <li>列表项2</li>
        ...
    </ol>
    ```

    ![image-20201125004704914](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201125004704914.png)

  + 自定义列表（重点）

    ```html
    <dl>
      <dt></dt>
      <dd></dd>
    </dl>
    ```
    
    s
    
    <img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201125005558916.png" alt="image-20201125005558916" style="zoom:50%;" />

+ 表单标签

  目的是为了收集用户信息  

  ![image-20201201231055466](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201201231055466.png)

  + 表单域 \<form>  是一个包含表单元素的区域，会把它范围内的表单元素信息提交给服务器。

    ![image-20201201232704413](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201201232704413.png)

  + 表单控件（元素）只有放到表单域里面，才能向服务器进行提交

    + \<input />  单标签

      ```html
      <input type='属性值' />
      ```

      <img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201201233642986.png" alt="image-20201201233642986" style="zoom:50%;" />

      注意：单选框和复选框的 name属性值要相同才能实现只能选一个和多个。

      ![image-20201202000226310](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201202000226310.png)
    
    + \<label> 标签为 input 元素定义标注（标签）
    
      ![image-20201202124124198](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201202124124198.png)
    
    + \<select> 下拉表单元素
    
      ```html
      <select>
        <option>选项1</option>
        <option>选项2</option>
        <option>选项3</option>
        ...
      </select>
      ```
    
      ![image-20201202114118067](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201202114118067.png)
    
    + textarea 文本域元素
    
      可以定义多行文本输入
    
      ![image-20201202120237624](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201202120237624.png)
    

+ \<hr>  分割线

## 特殊字符

一些特殊的符号很难或者不方便直接使用，此时我们用下面的符号来替代。

+ 空格、小于号、大于号

<img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201124173711871.png" alt="image-20201124173711871" style="zoom:50%;" />

# css

Cacading Style Sheets (层叠样式表)   也是一种标记语言

<img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201203005225199.png" alt="image-20201203005225199" style="zoom:50%;" />

<img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201203012107696.png" alt="image-20201203012107696" style="zoom:50%;" />

## 基础选择器

（由单个选择器组成)

+ 标签选择器

  选中页面中所有相同的标签

+ 类选择器

  口诀：==样式点定义 结构类调用== 一个或多个 开发最常用 

  <img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201203201718989.png" alt="image-20201203201718989" style="zoom:50%;" />

  <img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201203201603153.png" alt="image-20201203201603153" style="zoom:50%;" />

  多类名：

  <img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201203205401175.png" alt="image-20201203205401175" style="zoom:50%;" />

+ id选择器

  口诀: 样式#定义, 结构id调用, 只能调用一次, 别人切勿使用

  <img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201203205457584.png" alt="image-20201203205457584" style="zoom:50%;" />

  结构中用 id='nav' 来调用  

  ![image-20201203205905114](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201203205905114.png)

  ## 通配选择器

  <img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201204133331382.png" alt="image-20201204133331382" style="zoom:50%;" />


## 复合选择器

+ 后代选择器

  ```html
  元素1 元素2 { 样式声明 }
  ```

     元素1 和 元素2 可以是任意基础选择器

+ 子选择器

  ```html
  元素1 > 元素2 { 样式声明 } 
  ```

  ​	只能选择作为某元素的最近一级子元素。简单理解就是选亲儿子元素.

+ 并集选择器

  ```html
  元素1,元素2 { 样式声明 } 
  ```

  ​	任何形式的选择器都可以作为并集选择器的一部分，用 “ ，”分割

  ​	习惯逗号后换行，最后一个选择器后不需要加逗号

+ 伪类选择器

  + 链接伪类选择器 

    ![image-20201205110242243](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201205110242243.png)

    注意事项

    ![image-20201205111147768](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201205111147768.png)

    ![image-20201205112249149](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201205112249149.png)

  + ：focus  伪类选择器

    :focus 伪类选择器用于选取获得焦点的表单元素。 

    焦点就是光标，一般情况 \<input>  类表单元素才能获取，因此这个选择器也主要针对于表单元素来说。

    ```html
    input:focus {
     background-color:yellow;
    } 
    ```

## 字体属性

<img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201204173902651.png" alt="image-20201204173902651" style="zoom:50%;" />

​	**字体大小**

​	font-size: 20px;

​	标题标签\<p>比较特殊，需要单独指定文字大小，不能用\<body>选择器统一选	择。

​	**字体粗细**

<img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201204193813826.png" alt="image-20201204193813826" style="zoom:50%;" />

​	**文字样式**

<img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201204194324994.png" alt="image-20201204194324994" style="zoom:50%;" />

​	**字体复合属性**

 口诀：类粗大家（类型，粗细，大小，家族）

![image-20201204195101995](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201204195101995.png)

##文本属性

文本颜色

<img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201204200329092.png" alt="image-20201204200329092" style="zoom: 50%;" />

对齐文本

<img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201204200556568.png" alt="image-20201204200556568" style="zoom:50%;" />

==注意==：图片的居中，可以将图片标签看成特殊的文本，然后对**包含它的**标签用 text-align 来定义相关设定。

装饰文本

<img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201204202316712.png" alt="image-20201204202316712" style="zoom: 50%;" />

文本缩进

<img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201204202810613.png" alt="image-20201204202810613" style="zoom:50%;" />

行间距

<img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201204203042135.png" alt="image-20201204203042135" style="zoom:50%;" />

==注意==：行高后面也可以不写px单位，如下面的代表行高为 12*1.5 px，这样的话行高可以根据文字调整大小，在开发中比较常见。

<img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201205194253342.png" alt="image-20201205194253342" style="zoom:50%;" />

##css 的引入方式

<img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201204204341173.png" alt="image-20201204204341173" style="zoom:50%;" />

<img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201204204612552.png" alt="image-20201204204612552" style="zoom:50%;" />

<img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201204205134450.png" alt="image-20201204205134450" style="zoom:50%;" />

<img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201204205807070.png" alt="image-20201204205807070" style="zoom:50%;" />

## Emmet 语法

+ **快速生成HTML结构语法**

1. 生成标签 直接输入标签名 按tab键即可 比如 div 然后tab 键， 就可以生成 

2. 如果想要生成多个相同标签 加上 * 就可以了 比如 div*3 就可以快速生成3个div 

3. 如果有父子级关系的标签，可以用 > 比如 ul > li就可以了 
4. 如果有兄弟关系的标签，用 + 就可以了 比如 div+p 
5. 如果生成带有类名或者id名字的， 直接写 .demo 或者 #two tab 键就可以了 
6. 如果生成的div 类名是有顺序的， 可以用 自增符号 $ 
7. 如果想要在生成的标签内部写内容可以用 { } 表示

+ **快速生成CSS样式语法**

  CSS 基本采取简写形式即可

  ​	1. 比如 w200 按tab 可以 生成 width: 200px; 

  ​	2. 比如 lh26px 按tab 可以生成 line-height: 26px;

## 元素显示模式

+ 块元素

  常见的块元素有

  ![image-20201205115251305](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201205115251305.png)

  ① 比较霸道，自己独占一行。 

  ② 高度，宽度、外边距以及内边距都可以控制。 

  ③ 宽度默认是容器（父级宽度）的100%。

  ④ 是一个容器及盒子，里面可以放行内或者块级元素。

  ==注意==

  + 文字类的元素内不能使用块级元素 

  + \<p> 标签主要用于存放文字，因此 \<p> 里面不能放块级元素，特别是不能放 \<div>

  +  同理，\<h1>~\<h6> 等都是文字类块级标签，里面也不能放其他块级元素

+ 行内元素

  ![image-20201205115337907](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201205115337907.png)

+ 行内块元素

  ![image-20201205120258268](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201205120258268.png)

**元素显示模式转换**

1. 转换为块元素：display:block;

2. 转换为行内元素：display:inline; 
3. 转换为行内块：display: inline-block;

 ## snipaste

![image-20201205152249625](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201205152249625.png)

## css 的背景

+  背景颜色

  background-color:颜色值;

  默认值是 transparent （透明）

+  背景图片

  与直接用 \<img> 插入图片相比，背景图片更方便调整位置。

  background-image : none | url (url) 

![image-20201205165359061](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201205165359061.png)

+ 背景平铺

  ==页面元素既可以设置背景颜色也可以添加背景图片，只不过背景图片会压住背景颜色==

  默认情况是 repeat

  ![image-20201205165523058](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201205165523058.png)

+ 背景图片位置

   background-position: x y; 

![image-20201205171245780](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201205171245780.png)

1. 参数是方位名词 

   + 如果指定的两个值都是方位名词，则两个值前后顺序无关，比如 left top 和 top left 效果一致 

   + 如果只指定了一个方位名词，另一个值省略，则第二个值默认居中对齐 

2. 参数是精确单位 

   + 如果参数值是精确坐标，那么第一个肯定是 x 坐标，第二个一定是 y 坐标 
   + 如果只指定一个数值，那该数值一定是 x 坐标，另一个默认垂直居中 

3. 参数是混合单位 

   + 如果指定的两个值是精确单位和方位名词混合使用，则第一个值是 x 坐标，第二个值是 y 坐标

+ 背景图像固定（背景附着）

  background-attachment : scroll | fixed 

  ![image-20201205174541680](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201205174541680.png)

+ 背景复合写法

  没有特定的书写顺序,一般习惯约定顺序为：

  background: 背景颜色 背景图片地址 背景平铺 背景图像滚动 背景图片位置;

+ 背景颜色半透明

  CSS3 为我们提供了背景颜色半透明的效果。

  background: rgba(0, 0, 0, 0.3)；

  + 最后一个参数是 alpha 透明度，取值范围在 0~1之间 
  +  我们习惯把 0.3 的 0 省略掉，写为 background: rgba(0, 0, 0, .3); 
  + 注意：背景半透明是指**盒子背景半透明**，盒子里面的内容不受影响 
  + CSS3 新增属性，是 IE9+ 版本浏览器才支持的 
  + 但是现在实际开发，我们不太关注兼容性写法了,可以放心使用

## css的三大特性

层叠性、继承性、优先级

+ 层叠性

  ![image-20201205193307957](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201205193307957.png)

+ 继承性

  ![image-20201205193509901](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201205193509901.png)

  ![image-20201205193542651](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201205193542651.png)

  ==只是继承某些样式（跟文字相关的会继承）==

+ 优先级

  <img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201205194719504.png" alt="image-20201205194719504" style="zoom:50%;" />

  ![image-20201212095309383](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201212095309383.png)

  **类选择器、属性选择器、伪类选择器，权重为 10**

  **伪元素选择器权重为1**
  
  复合选择器会有权重叠加的问题
  
  ![image-20201205202407826](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201205202407826.png)

## css盒子模型

+ 盒子模型组成

  border     边框 

  content    内容 

  padding   内边距 

  margin     外边距 

<img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201205211142904.png" alt="image-20201205211142904" style="zoom: 67%;" />

+ border 边框

  ```css
  border : border-width || border-style || border-color 
  ```

  ![image-20201205211505036](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201205211505036.png)

  边框样式 border-style 可以设置如下值： 

  ​	none：没有边框即忽略所有边框的宽度（默认值） 

  ​	solid：边框为单实线(最为常用的)  

  ​	dashed：边框为虚线 

  ​	dotted：边框为点线

  边框的复合写法：

     border: 1px solid red; 没有顺序 

  边框分开写法：

     border-top: 1px solid red; /* 只设定上边框， 其余同理 */

  **表格的细线边框**

  ```css
  border-collapse:collapse; 
  ```

  collapse 单词是合并的意思，表示相邻边框合并在一起
  
  **边框会影响盒子实际大小**
  
  边框会额外增加盒子的实际大小。因此我们有两种方案解决: 
  
  1. 测量盒子大小的时候,不量边框. 
  2. 如果测量的时候包含了边框,则需要 width/height 减去边框宽度

+ padding   内边距 （会影响盒子的实际大小）

  但是如何盒子本身没有指定width/height属性, 则此时padding不会撑开盒子大小.

  ![image-20201205235747951](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201205235747951.png)
  
  ![image-20201205235841502](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201205235841502.png)
  
+ margin     外边距 

  ![image-20201206104039256](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201206104039256.png)

  margin 简写方式代表的意义跟 padding 完全一致。

  外边距可以让块级盒子水平居中，但是必须满足 两个条件：

   ① 盒子必须指定了宽度（width）。

   ② 盒子左右的外边距都设置为 auto 。

  ==注意==：以上方法是让**块级**元素水平居中，**行内元素**或者**行内块元素**水平居中给其父元素添加 text-align:center 即可。（因为块元素会占据一整行，外边距设置为auto之后会进行平分，从而达到居中的效果）

  **外边距合并**

  1. **相邻块元素垂直外边距的合并**

  ![image-20201206111010273](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201206111010273.png)

  2. **嵌套块元素垂直外边距的塌陷**

  ![image-20201206111359504](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201206111359504.png)

  还有其他方法，比如浮动、固定，绝对定位的盒子不会有塌陷问题，后面咱们再总结。

  ==浮动的盒子不会有外边距合并的问题==

+ 清除内外边距

  网页元素很多都带有默认的内外边距，而且不同浏览器默认的也不一致。因此我们在布局前，首先要清除下网 页元素的内外边距。

```html
* {
 		padding:0; /* 清除内边距 */
		margin:0; /* 清除外边距 */
 	}

```

​	**注意**：行内元素为了照顾兼容性，尽量只设置左右内外边距，不要设置上下内外边距。但是转换为块级和行内块元素就可以了

## 圆角边框

语法：

```css
border-radius:length; 
```

+ 参数值可以为数值或百分比的形式 
+ 如果是正方形，想要设置为一个圆，把数值修改为高度或者宽度的一半即可，或者直接写为 50% 
+ 该属性是一个简写属性，可以跟四个值，分别代表左上角、右上角、右下角、左下角 
+ 分开写：border-top-left-radius、border-top-right-radius、border-bottom-right-radius 和 border-bottom-left-radius 
+ 兼容性 ie9+ 浏览器支持, 但是不会影响页面布局,可以放心使用.

## 盒子阴影

语法：

```html
box-shadow: h-shadow v-shadow blur spread color inset; 
```

<img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201206163054925.png" alt="image-20201206163054925" style="zoom:50%;" />

模糊距离（blur）是指阴影的虚实，越大越模糊，0 的时候为实的

阴影的尺寸（spread）影子的大小 

==注意==： 

1. 默认的是外阴影(outset), 但是不可以写这个单词,否则造成阴影无效 
2. 盒子阴影不占用空间，不会影响其他盒子排列。

## 文字阴影

语法： 

```css
text-shadow: h-shadow v-shadow blur color;
```

![image-20201206164028886](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201206164028886.png)

## css浮动

网页布局的本质——用 CSS 来摆放盒子。 把盒子摆放到相应位置.

CSS 提供了三种传统布局方式(简单说,就是盒子如何进行排列顺序)：

+ 普通流（标准流） 

+ 浮动

+ 定位

  ![image-20201206165043923](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201206165043923.png)

**为什么需要浮动？**

总结： 有很多的布局效果，标准流没有办法完成，此时就可以利用浮动完成布局。 因为浮动可以改变元素标签默认的排列方式. 

浮动最典型的应用：可以让多个块级元素一行内排列显示。

==网页布局第一准则==：**多个块级元素纵向排列找标准流，多个块级元素横向排列找浮动。**

**浮动定义**：

![image-20201206170019766](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201206170019766.png)

**浮动特性（重难点）**：

1. ==浮动元素会脱离标准流(脱标)==

   脱离标准普通流的控制（浮） 移动到指定位置（动）, （俗称脱标）

   浮动的盒子**不再保留原先的位置**

   ![image-20201206172409940](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201206172409940.png)

2. 浮动的元素会一行内显示并且元素顶部对齐  

   **注意**： 与行内块不同，浮动的元素是互相贴靠在一起的（不会有缝隙），如果父级宽度装不下这些浮动的盒子， 多出的盒子会另起一行对齐。

3. 浮动的元素会具有行内块元素的特性.

   任何元素都可以浮动。不管原先是什么模式的元素，添加浮动之后具有**行内块元素**相似的特性。 

   + 如果块级盒子没有设置宽度，默认宽度和父级一样宽，但是添加浮动后，它的大小根据内容来决定 
   + 浮动的盒子中间是没有缝隙的，是紧挨着一起的 
   + 行内元素同理

==浮动元素不同，只会压住它下面标准流的盒子，但是不会压住下面标准流盒子里面的文字（图片）==

**浮动元素经常和标准流父级搭配使用**

​	为了约束浮动元素位置, 我们网页布局一般采取的策略是: 

​	==先用标准流的父元素排列上下位置, 之后内部子元素采取浮动排列左右位置，符合网页布局第一准侧.==

![image-20201206180313119](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201206180313119.png)

==网页布局第二准侧==：先设置盒子的大小, 之后设置盒子的位置.

![image-20201206203355404](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201206203355404.png)

## 清除浮动

由于父级盒子很多情况下，不方便给高度，但是子盒子浮动又不占有位置，最后父级盒子高度为 0 时，就会影响下面的标准流盒子

![image-20201206204659932](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201206204659932.png)

由于浮动元素不再占用原文档流的位置，所以它会对后面的元素排版产生影响

语法：

`选择器{clear:属性值;}` 

![image-20201206205756703](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201206205756703.png)

**==清除浮动方法==**

1. **额外标签法也称为隔墙法，是 W3C 推荐的做法。**

   ![image-20201206211020829](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201206211020829.png) 

2. **父级添加 overflow 属性** 

   ​	可以给父级添加 overflow 属性，将其属性值设置为 **hidden**、 auto 或 scroll 。 子不教，父之过，注意是给**父元素**添加代码 

   ​	优点：代码简洁 

   ​	缺点：无法显示溢出的部分

3. **父级添加after伪元素** 

   :after 方式是额外标签法的升级版。也是给**父元素**添加

   ```css
   .clearfix:after {
    	content: "";
    	display: block;
    	height: 0;
    	clear: both;
    	visibility: hidden;
   }
   .clearfix { 
     /* IE6、7 专有 */
    	*zoom: 1;
   }
   ```

   优点：没有增加标签，结构更简单 

   缺点：照顾低版本浏览器 

   代表网站： 百度、淘宝网、网易等

4. **父级添加双伪元素**

   也是给给**父**元素添加

   ```css
   .clearfix:before,
   .clearfix:after {
    	content:"";
    	display:table;
   }
   
   .clearfix:after {
    	clear:both;
   }
   
   .clearfix {
     /* IE6、7 专有 */
    	*zoom:1;
   }
   ```

   优点：代码更简洁 

   缺点：照顾低版本浏览器

   代表网站：小米、腾讯等

## PS切图

![image-20201206213005835](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201206213005835.png)

![image-20201206213605126](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201206213605126.png)

![image-20201206214321134](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201206214321134.png)

![image-20201206215521623](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201206215521623.png)

## CSS 属性书写顺序(重点)

建议遵循以下顺序：

1. 布局定位属性：display / position / float / clear / visibility / overflow（建议 display 第一个写，毕竟关系到模式）
2. 自身属性：width / height / margin / padding / border / background
3. 文本属性：color / font / text-decoration / text-align / vertical-align / white- space / break-word 
4. 其他属性（CSS3）：content / cursor / border-radius / box-shadow / text-shadow / background:linear-gradient …

```css
.jdc {
  display: block;
  position: relative;
  float: left;
  width: 100px;
  height: 100px;
  margin: 0 10px;
  padding: 20px 0;
  font-family: Arial, 'Helvetica Neue', Helvetica, sans-serif;
  color: #333;
  background: rgba(0,0,0,.5);
  border-radius: 10px;
} 
```

为了提高网页制作的效率，布局时通常有以下的**布局流程**： 

1. 必须确定页面的版心（可视区），我们测量可得知。 
2. 分析页面中的行模块，以及每个行模块中的列模块。其实页面布局，就是一行行罗列而成的。 
3. 制作 HTML 结构。我们还是遵循，先有结构，后有样式的原则。结构永远最重要。 
4. 开始运用盒子模型的原理，通过 DIV+CSS 布局来控制网页的各个模块。

## CSS 定位

**为什么需要定位**

1. **浮动**可以让多个块级盒子一行没有缝隙排列显示， 经常用于横向排列盒子。 
2. **定位**则是可以让盒子自由的在某个盒子内移动位置或者固定屏幕中某个位置，并且可以压住其他盒子。

**定位 = 定位模式 + 边偏移**

![image-20201208211926115](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201208211926115.png)

![image-20201208193953977](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201208193953977.png)

**2. 边偏移** 

边偏移就是定位的盒子移动到最终位置。有 top、bottom、left 和 right 4 个属性。

==注意==：如果一个盒子既有left属性也有right属性，则默认会执行left属性，同理top bottom会执行 top。

**静态定位 static（了解）**

![image-20201208194421874](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201208194421874.png)

**相对定位 relative（重要）**

![image-20201208194916477](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201208194916477.png)

**绝对定位 absolute（重要）**

![image-20201208200538618](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201208200538618.png)

所以绝对定位是脱离标准流的

==子绝父相==

① 子级绝对定位，不会占有位置，可以放到父盒子里面的任何一个地方，不会影响其他的兄弟盒子。 

② 父盒子需要加定位限制子盒子在父盒子内显示。 

③ 父盒子布局时，需要占有位置，因此父亲只能是相对定位。

当然，子绝父相不是永远不变的，如果父元素不需要占有位置，子绝父绝也会遇到。

**固定定位 fixed （重要）**

![image-20201208203923291](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201208203923291.png)

因为固定定位跟父元素没有关系，它以屏幕为准

==固定定位小技巧： 固定在版心右侧位置。==

小算法：

1. 让固定定位的盒子 left: 50%. 走到浏览器可视区（也可以看做版心） 的一半位置。 
2. 让固定定位的盒子 margin-left: 版心宽度的一半距离。 多走版心宽度的一半位置，就可以让固定定位的盒子贴着版心右侧对齐了。

定位元素如果设置了top left，margin top,left会使盒子按照定位后的位置移动

**粘性定位 sticky（了解）**

粘性定位可以被认为是相对定位和固定定位的混合。 Sticky 粘性的

![image-20201208211649916](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201208211649916.png)

**定位叠放次序 z-index**

![image-20201208213443288](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201208213443288.png)

## 定位的拓展

**绝对定位的盒子居中**

加了绝对定位和固定定位的盒子不能通过 margin:0 auto 水平居中，但是可以通过以下计算方法实现水平和垂直居中。

 ① left: 50%;：让盒子的左侧移动到父级元素的水平中心位置。 

② margin-left: -100px;：让盒子向左移动自身宽度的一半

**定位特殊特性**

绝对定位和固定定位也和浮动类似。

1. 行内元素添加绝对或者固定定位，可以直接设置高度和宽度。 
2. 块级元素添加绝对或者固定定位，如果不给宽度或者高度，默认大小是内容的大小。

**脱标的盒子不会触发外边距塌陷**

浮动元素、绝对定位(固定定位）元素的都不会触发外边距合并的问题。

**绝对定位（固定定位）会完全压住盒子**

浮动元素不同，只会压住它下面标准流的盒子，但是不会压住下面标准流盒子里面的文字（图片） 

但是绝对定位（固定定位） 会压住下面标准流所有的内容。 

浮动之所以不会压住文字，因为浮动产生的目的最初是为了做文字环绕效果的。 文字会围绕浮动元素

==理解==：绝对定位跟固定定位是不占有原先的位置的所以之前的位置就腾出去然后被盖住了

 ## 元素的显示与隐藏

**display 属性**

display 属性用于设置一个元素应如何显示。 

+  display: none ；隐藏对象 
+ display：block ；除了转换为块级元素之外，同时还有显示元素的意思 

==display 隐藏元素后，不再占有原来的位置。==

后面应用及其广泛，搭配 JS 可以做很多的网页特效。

**visibility 可见性**

visibility 属性用于指定一个元素应可见还是隐藏。 

+ visibility：visible ; 元素可视 
+ visibility：hidden; 元素隐藏 

==visibility 隐藏元素后，继续占有原来的位置。==

如果隐藏元素想要原来位置， 就用 visibility：hidden 

如果隐藏元素不想要原来位置， 就用 display：none (用处更多 重点）

**overflow 溢出**

![image-20201209213109775](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201209213109775.png)

## 精灵图

（sprites）也叫雪碧图

使用精灵图核心总结： 

1. 精灵图主要针对于小的背景图片使用。 
2. 主要借助于背景位置来实现---background-position 。 
3.  一般情况下精灵图都是负值。（千万注意网页中的坐标： x轴右边走是正值，左边走是负值， y轴同理。）

## 字体图标

字体图标使用场景： 主要用于显示网页中通用、常用的一些小图标。

精灵图是有诸多优点的，但是缺点很明显。

1. 图片文件还是比较大的。 
2. 图片本身放大和缩小会失真。
3. 一旦图片制作完毕想要更换非常复杂。 

此时，有一种技术的出现很好的解决了以上问题，就是字体图标 iconfont。 字体图标可以为前端工程师提供一种方便高效的图标使用方式，展示的是**图标**，本质属于**字体**。

==fontawesome==

**方法一**：通过类

图标字体（iconfont）

        - 在网页中经常需要使用一些图标，可以通过图片来引入图标
            但是图片大小本身比较大，并且非常的不灵活
        - 所以在使用图标时，我们还可以将图标直接设置为字体，
            然后通过font-face的形式来对字体进行引入
        - 这样我们就可以通过使用字体的形式来使用图标

​    fontawesome 使用步骤
​        1.下载 https://fontawesome.com/
​        2.解压
​        3.将css和webfonts移动到项目中
​        4.将all.css引入到网页中
​        5.使用图标字体

        - 直接通过类名来使用图标字体
            class="fas fa-bell"
            class="fab fa-accessible-icon"

```html
<i class="fas fa-bell" style="font-size:80px; color:red;"></i>
<i class="fas fa-bell-slash"></i>
<i class="fab fa-accessible-icon"></i>
<i class="fas fa-otter" style="font-size: 160px; color:green;"></i>
```



**方法二**:通过伪元素

```css
li::before{
            /* 
                通过伪元素来设置图标字体
                    1.找到要设置图标的元素通过before或after选中
                    2.在content中设置字体的编码
                    3.设置字体的样式
                        fab
                        font-family: 'Font Awesome 5 Brands';

                        fas
                        font-family: 'Font Awesome 5 Free';
                        font-weight: 900; 

            */
            content: '\f1b0';
            /* font-family: 'Font Awesome 5 Brands'; */
            font-family: 'Font Awesome 5 Free';
            font-weight: 900; 
            color: blue;
            margin-right: 10px;
        }
```

**方法三**：通过实体

通过实体来使用图标字体：
            &#x图标的编码;

```html
 <span class="fas">&#xf0f3;</span>
```

==icomoon==

http://icomoon.io

![image-20201210180948575](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201210180948575.png)

![image-20201210181003765](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201210181003765.png)

![image-20201210181026121](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201210181026121.png)

![image-20201210181453902](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201210181453902.png)

![image-20201210181515436](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201210181515436.png)

![image-20201210181531972](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201210181531972.png)

## CSS 三角

![image-20201210192511380](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201210192511380.png)

##  CSS 用户界面样式

**鼠标样式 cursor**

```html
li {cursor: pointer; }
```

![image-20201210200355582](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201210200355582.png)

**轮廓线 outline**

![image-20201210200548264](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201210200548264.png)

**防止拖拽文本域 resize**

实际开发中，我们文本域右下角是不可以拖拽的。

```css
textarea{ resize: none;}
```

\<textarea>\</textarea>最好写在一行上，否则光标定过去的时候会有空白

**vertical-align 属性应用**

默认是基线对齐

![image-20201210202445659](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201210202445659.png)

![image-20201210202520327](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201210202520327.png)

![image-20201210203059733](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201210203059733.png)

==解决图片底部默认空白缝隙问题==

bug：图片底侧会有一个空白缝隙，原因是行内块元素会和文字的基线对齐。

![image-20201210205927530](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201210205927530.png)

![image-20201210205939972](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201210205939972.png)

主要解决方法有两种： 

1. 给图片添加 vertical-align:middle | top| bottom 等。 （提倡使用的） 
2. 把图片转换为**块级**元素 display: block;

## 溢出的文字省略号显示

**1. 单行文本溢出显示省略号--必须满足三个条件**

![image-20201210210731050](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201210210731050.png)

**2.多行文本溢出显示省略号**

![image-20201210211109974](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201210211109974.png)

## 常见布局技巧

**1. margin负值运用**

下面案例需要实现的效果，盒子与盒子之间有一个边框，当鼠标移入其中某一个盒子是该盒子的边框颜色改变。

![image-20201210212913076](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201210212913076.png)

**2. 文字围绕浮动元素**

![image-20201211140807252](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201210215332840.png)

**3. 行内块巧妙运用**

如果给行内块的父元素设置 text-align ：center ，可以父元素里面的块元素实现居中对齐

![image-20201210235050724](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201210235050724.png)

**4. CSS 三角强化**

![image-20201211000757896](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201211000757896.png)

## CSS 初始化

不同浏览器对有些标签的默认值是不同的，为了消除不同浏览器对HTML文本呈现的差异，照顾浏览器的兼 容，我们需要对CSS 初始化

京东做法：

```css
/* 把我们所有标签的内外边距清零 */
* {
    margin: 0;
    padding: 0;
  	/*css3 盒子模型*/
  	box-sizing: border-box;
}
/* em 和 i 斜体的文字不倾斜 */
em,
i {
    font-style: normal
}
/* 去掉li 的小圆点 */
li {
    list-style: none
}

img {
    /* border 0 照顾低版本浏览器 如果 图片外面包含了链接会有边框的问题 */
    border: 0;
    /* 取消图片底侧有空白缝隙的问题 */
    vertical-align: middle
}

button {
    /* 当我们鼠标经过button 按钮的时候，鼠标变成小手 */
    cursor: pointer
}

a {
    color: #666;
    text-decoration: none
}

a:hover {
    color: #c81623
}

button,
input {
    /* "\5B8B\4F53" 就是宋体的意思 这样浏览器兼容性比较好 */
    font-family: Microsoft YaHei, Heiti SC, tahoma, arial, Hiragino Sans GB, "\5B8B\4F53", sans-serif
}

body {
    /* CSS3 抗锯齿形 让文字显示的更加清晰 */
    -webkit-font-smoothing: antialiased;
    background-color: #fff;
    font: 12px/1.5 Microsoft YaHei, Heiti SC, tahoma, arial, Hiragino Sans GB, "\5B8B\4F53", sans-serif;
    color: #666
}

.hide,
.none {
    display: none
}
/* 清除浮动 */
.clearfix:after {
    visibility: hidden;
    clear: both;
    display: block;
    content: ".";
    height: 0
}

.clearfix {
    *zoom: 1
}
```

# HTML5 和 CSS3 提高

## HTML5 的新特性

HTML5 的新增特性主要是针对于以前的不足，增加了一些新的标签、新的表单和新的表单属性等。

 这些新特性都有兼容性问题，基本是 IE9+ 以上版本的浏览器才支持，如果不考虑兼容性问题，可以大量使用这 些新特性。

**H5 自定义数据属性**: HTML5规定可以为元素添加非标准的属性，但要添加前缀data-, 目的是为元素提供与渲染无关的信息，或者提供语义信息。

```html
 <div id="myDiv" data-appId="12345" data-myname="Nicholas"></div>  
```

添加自定义属性之后，可以通过元素的dataset属性来访问自定义属性的值。

**HTML5 新增的语义化标签**

![image-20201211153351955](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201211153351955.png)

**HTML5 新增的多媒体标签**

1. **==视频\<video>==**

![image-20201211161500038](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201211161500038.png)

![image-20201211161416267](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201211161416267.png)

![image-20201211161526645](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201211161526645.png)

2. **==音频\<audio>==**

![image-20201211162203114](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201211162203114.png)

![image-20201211162402223](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201211162402223.png)

![image-20201211162412370](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201211162412370.png)

对于谷歌，我们可以给视频标签添加 muted 属性来静音播放视频，音频不可以（可以通过JavaScript解决）

**HTML5 新增的 input 类型**

![image-20201211162807526](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201211162807526.png)

**HTML5 新增的表单属性**

![image-20201211164924264](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201211164924264.png)

## CSS3 的新特性

新增的CSS3特性有兼容性问题，ie9+才支持

移动端支持优于 PC 端 

不断改进中 

应用相对广泛 

现阶段主要学习：新增选择器和盒子模型以及其他特性

**1.属性选择器**

![image-20201211233433610](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201211233433610.png)

正则表达式也是用 ^ $

==注意：类选择器、属性选择器、伪类选择器，权重为 10。==

![image-20201211234445395](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201211234445395.png)

**2.结构伪类选择器**

![image-20201212000350241](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201212000350241.png)

==xx:nth-child(n) 里面的 xx 指的就是子元素==

==nth-child（n） 选择某个父元素的一个或多个特定的子元素（重点）==

n 可以是数字，关键字和公式 

n 如果是数字，就是选择第 n 个子元素， 里面数字从1开始… 

n 可以是关键字：even 偶数，odd 奇数 

n 可以是**公式**：常见的公式如下 ( 如果n是公式，则从0开始计算，但是第 0 个元素或者超出了元素的个数会被忽略 )

![image-20201212001715250](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201212001715250.png)

==区别==

1. nth-child 是在所有孩子里面寻找第 n 个孩子，如果该孩子与 E 匹配，则选择成功，否则选不上。 
2. nth-of-type 先去匹配E ，然后再找到 E 中的第n个孩子。

**3.伪元素选择器（重点）**

==注意是在内部创建的伪元素，是子元素！==

伪元素选择器可以帮助我们利用CSS创建新标签元素，而不需要HTML标签，从而简化HTML结构。

![image-20201212095025925](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201212095025925.png)

![image-20201212103725313](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201212103725313.png)

![image-20201212103732123](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201212103732123.png)

![image-20201212103807089](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201212103807089.png)

<img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201212104926524.png" alt="image-20201212104926524" style="zoom:50%;" />

<img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201212105236350.png" alt="image-20201212105236350" style="zoom:50%;" />

**4.CSS3 2D转换**

转换（transform）是CSS3中具有颠覆性的特征之一，可以实现元素的位移、旋转、缩放等效果

+ 移动：translate

  移动盒子位置的方法：定位   盒子的外边距   2d转换移动

  ![image-20201224161453550](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201224161453550.png)

  ==不会影响到其他元素的位置==（类似于相对定位）

  百分比是相对于自身来计算的，因此可以利用这个特性来设置一个盒子水品居中或者高度居中。

+ 旋转：rotate

  ![image-20201224165130641](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201224165130641.png)

  应用：

  ![image-20201224171916667](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201224171916667.png)

  ```css
  p::before {
              content: '';
              position: absolute;
              right: 20px;
              top: 10px;
              width: 10px;
              height: 10px;
              border-right: 1px solid #000;
              border-bottom: 1px solid #000;
              transform: rotate(45deg);
  }
  
  ```

  2D 转换中心点 transform-origin 参数可以百分比、像素或者是方位名词

  ![image-20201224172611430](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201224172611430.png)

+ 缩放： 

  ![image-20201224200239584](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201224200239584.png)

  也是用 transform-origin 来设置转换中心点

+ 2D 转换综合写法

  ==注意==

  1. 同时使用多个转换，其格式为：transform: translate() rotate() scale() ...等，
  2. 其顺序会影转换的效果。（先旋转会改变坐标轴方向）
  3. ==**当我们同时有位移和其他属性的时候，记得要将位移放到最前**==（因为如果先旋转的话坐标系也会跟着旋转）

**5.css3 动画**

 **动画（animation）**是CSS3中具有颠覆性的特征之一，可通过设置多个节点来精确控制一个或一组动画，常用来实现复杂的动画效果。
相比较过渡，动画可以实现更多变化，更多控制，连续自动播放等效果。

制作动画分为两步：

1. 先定义动画
2. 再使用（调用）动画

keyframes  关键帧

![image-20201224212050659](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201224212050659.png)

动画序列：

+ 0% 是动画的开始，100% 是动画的完成。这样的规则就是动画序列。
+ 在 @keyframes 中规定某项 CSS 样式，就能创建由当前样式逐渐改为新样式的动画效果。
+ 动画是使元素从一种样式逐渐变化为另一种样式的效果。您可以改变任意多的样式任意多的次数。
+ 请用百分比来规定变化发生的时间，或用关键词 "from" 和 "to"，等同于 0% 和 100%。

![image-20201224212238061](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201224212238061.png)

![image-20201224213402206](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201224213402206.png)

说明：

animation-timing-function

![image-20201225014130750](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201225014130750.png)

steps(n) 就是分 n 步来完成动画，步与步之间不会有过渡。 

animation-iteration-count：infinite（播放无限次）

动画简写属性：

animation：动画名称 持续时间 运动曲线 何时开始 播放次数 是否反方向  动画起始或者结束的状态;

+ 简写属性里面不包含 animation-play-state 
+ 暂停动画：animation-play-state:   puased;   经常和鼠标经过等其他配合使用
+ 想要动画走回来 ，而不是直接跳回来：animation-direction   ：  alternate
+ 盒子动画结束后，停在结束位置：  animation-fill-mode  ：   forwards 

opacity: 1;  透明度，默认为1

**6.CSS3 3D转换**

x轴：水平向右      注意： x 右边是正值，左边是负值 
y轴：垂直向下      注意： y 下面是正值，上面是负值
z轴：垂直屏幕      注意： 往外面是正值，往里面是负值 

+ 3D位移: translate3d(x,y,z)

  ![image-20201225132355820](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201225132355820.png)

  xyz 不能省略，没有就写 0 

+ 透视: perspective

  ==透视写到被观察元素的**父**盒子上面==

  可以先将父盒子设置为透视之后，其子盒子就可以设置不同的 translateZ 值

  透视的单位是像素，可以理解为眼睛到屏幕的距离，**近大远小**

  ![image-20201225175448465](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201225175448465.png)

+ 3D旋转: rotate3d(x,y,z)

  transform:rotateX(45deg)：沿着x轴正方向旋转 45度
  transform:rotateY(45deg) ：沿着y轴正方向旋转 45deg
  transform:rotateZ(45deg) ：沿着Z轴正方向旋转 45deg
  transform:rotate3d(x,y,z,deg)： 沿着自定义轴旋转 deg为角度（了解即可）

  ![image-20201225183339187](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201225183339187.png)

  ![image-20201225183805419](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201225183805419.png)

+ 3D呈现 transform-style

  ![image-20201225190219480](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201225190219480.png)

将这个属性设置为 preserve-3d 之后，父盒子里面的多个子盒子满足 3d 效果，如上边右图所示。

而 perspective 是透视，是为了显示出近大远小的效果

**CSS3 盒子模型**

box-sizing

![image-20201212125444047](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201212125444047.png)

<img src="D:\学习文件\笔记OLY\html css\html-css.assets\image-20201212125537175.png" alt="image-20201212125537175" style="zoom:50%;" />

**7.浏览器私有前缀**

浏览器私有前缀是为了兼容老版本的写法，比较新版本的浏览器无须添加。

1. 私有前缀

   -moz-：代表 firefox 浏览器私有属性
   -ms-：代表 ie 浏览器私有属性
   -webkit-：代表 safari、chrome 私有属性
   -o-：代表 Opera 私有属性

2.  提倡的写法(先写私有的，再写总的)

   ```css
   -moz-border-radius: 10px; 
   -webkit-border-radius: 10px; 
   -o-border-radius: 10px; 
   border-radius: 10px;
   ```

**8.CSS3 其他特性（了解）**

1. 图片变模糊

![image-20201212130054735](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201212130054735.png)

1. 计算盒子宽度 width: calc 函数

   CSS3 calc 函数: calc() 

   此CSS函数让你在声明CSS属性值时执行一些计算。

   ![image-20201212130420477](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201212130420477.png)

**CSS3 过渡（重点）**

transition

==在经常和 :hover 一起 搭配使用==

![image-20201212131302523](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201212131302523.png)

如果想要写多个属性，利用逗号进行分割 或者 属性写 all 就可以了

js 检测过渡完成事件 transitionend

# 品优购项目

## 网站 favicon 图标![image-20201216130508153](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201216130508153.png)

比特虫：http://www.bitbug.net/

![image-20201216130528347](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201216130528347.png)

![image-20201216130539602](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201216130539602.png)

![image-20201216131049829](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201216131049829.png)

引入的代码在比特虫里面复制即可，无需记忆

## 网站TDK三大标签SEO优化

SEO（Search Engine Optimization）汉译为搜索引擎优化

SEO 的目的是**对网站进行深度的优化**，从而帮助网站获取免费的流量，进而在搜索引擎上提升网站的排名，提高网站的知名度。  **tdk**

![image-20201219000611866](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201219000611866.png)

```html
<title>品优购商城-综合网购首选-正品低价、品质保障、配送及时、轻松购物!</title>
  <!-- 网站说明 -->
  <meta name="description"
    content="京东JD.COM-专业的综合网上购物商城,销售家电、数码通讯、电脑、家居百货、服装服饰、母婴、图书、食品等数万个品牌优质商品.便捷、诚信的服务，为您提供愉悦的网上购物体验!" />
  <!-- 关键字 -->
  <meta name=" keywords" content="网上购物,网上商城,手机,笔记本,电脑,MP3,CD,VCD,DV,相机,数码,配
件,手表,存储卡,京东" />
```

## LOGO SEO 优化

1. logo 里面首先放一个 h1 标签，目的是为了提权，告诉搜索引擎，这个地方很重要。 

2. h1 里面再放一个链接，可以返回首页的，把 logo 的背景图片给链接即可。 

3. 为了搜索引擎收录我们，我们链接里面要放文字（网站名称），但是文字不要显示出来。

   方法1：text-indent 移到盒子外面（text-indent: -9999px) ，然后 overflow:hidden ，淘宝的做法。 

   方法2：直接给 font-size: 0; 就看不到文字了，京东的做法。

4. 最后给链接一个 title 属性，这样鼠标放到 logo 上就可以看到提示

   

## 常用模块类名命名

![image-20201219144916582](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201219144916582.png)

## 将自己的网站上传到远程服务器

注意：一般稳定的服务器都是需要收费的。 比如：阿里云 这里给大家推荐一个免费的远程服务器（免费空间） http://free.3v.do/ 

1. 去免费空间网站注册账号。
2. 记录下主机名、用户名、密码、域名。
3. 利用 cutftp 软件 上传网站到远程服务器。
4. 在浏览器中输入域名，即可访问我们的品优购网站了。

# 移动端

 ## 视口

视口（ viewport）就是浏览器显示页面内容的屏幕区域。视口可以分为布局视口、视觉视口和理想视口

![image-20201228001109005](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201228001109005.png)

![image-20201228001229721](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201228001229721.png)

![image-20201228001402347](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201228001402347.png)

![image-20210104203539077](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210104203539077.png)

<meta name="viewport" content="width=device-width，user-scalable=no,initial-scale=1.0，maximum-scale=1.0,minimum-scale=1.0">

![image-20210104204019542](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210104204019542.png)

## 二倍图

![image-20201228093949408](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201228093949408.png)

PC端和早前的手机屏幕/普通手机屏幕：1 css像素=1物理像素的
Retina(视网膜屏幕)是一种显示技术，可以将把更多的物理像素点压缩至一块屏幕里，从而达到更高的分辨率，并提高屏幕显示的细腻程度.

==可以理解为1px在手机（例如iPhone8）中实际占两个物理像素，但是在谷歌的手机模拟中会把手机宽度调整为开发尺寸375（实际上是750物理像素）==

![image-20201228095318030](D:\学习文件\笔记OLY\html css\html-css.assets\image-20201228095318030.png)

**3.3 背景缩放 background-size**

![image-20210104192659682](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210104192659682.png)

注：

只写一个参数代表的是宽度，高度会等比例缩放；

百分比是相对于父盒子来说的；

![image-20210104211230015](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210104211230015.png)

## 移动端开发

![image-20210104211614144](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210104211614144.png)

![image-20210104212235877](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210104212235877.png)

css初始化：normalize.css（推荐使用）

官网网址：http://necolas.github.io/normalize.css/

**设置视口标签以及引入初始化样式**

```
<meta name="viewport" content="width=device-width,user-scalable=no,initial-scale=1.0,maximum-scale=1.0,minimum-scale=1.0">
<link rel="stylesheet" href="css/normalize.css">
<link rel="stylesheet" href="css/index.css">
```

**常用初始化样式**

```css
body {
max-width: 540px;
min-width: 320px;
margin: 0 auto;
font: normal 14px/1.5 Tahoma, "Lucida Grande", verdana, "MicrosoftYahei", STxihei,hei;
color: #000;
background: #f2f2f2;
overflow-x: hidden;
-webkit-tap-highlight-color: transparent;
}

```

**移动端特殊样式**

![image-20210104225657337](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210104225657337.png)

```
/*点击高亮我们需要清除清除  设置为transparent 完成透明*/
* {
    -webkit-tap-highlight-color: transparent;
}

/*在移动端浏览器默认的外观在iOS上加上这个属性才能给按钮和输入框自定义样式*/
input {
    -webkit-appearance: none;
}

/*禁用长按页面时的弹出菜单*/
img,
a {
    -webkit-touch-callout: none;
}
```

**移动端技术选型**

![image-20210104231553858](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210104231553858.png)

##流式布局（百分比布局）

![image-20210105132723887](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210105132723887.png)

max-width最大宽度（ max-height最大高度)

min-width最小宽度（ min-height最小高度)

用来保证盒子的尺寸在一个合理的尺寸范围内

## flex 弹性布局

![image-20210126185653434](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210126185653434.png)

![image-20210127145904497](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210127145904497.png)

采用Flex布局的元素，称为Flex**容器**（flex container )，简称"容器"。它的所有子元素自动成为容器成员，称为Flex项目( flex item )，简称"**项目**"。

总结flex布局原理:
就是通过给**父盒子**添加flex属性，来控制**子盒子**的位置和排列方式

在flex布局中，是分为主轴和侧轴两个方向，同样的叫法有︰行和列、x轴和y轴

![image-20210127151338263](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210127151338263.png)

+ **常见父项属性**

  以下由6个属性是对父元素设置的
  flex-direction :设置主轴的方向

  ![image-20210127151619397](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210127151619397.png)

  justify-content :设置**主轴**上的子元素排列方式

  ![image-20210127151946838](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210127151946838.png)

  flex-wrap :设置子元素是否换行

  >    flex布局中，默认的子元素是不换行的，如果装不开，会缩小子元素的宽度，放到父元素里面

  ![image-20210127153251128](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210127153251128.png)

  ）
  align-items :设置侧轴上的子元素排列方式(单行)

  ![image-20210127153836410](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210127153836410.png)

  > ​    stretch: 如果子元素没有设置高度，长度默认拉升为父元素一样的高度。 

  align-content:设置侧轴上的子元素的排列方式(多行）

  ![image-20210127155539529](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210127155539529.png)`align-content和align-items区别`

  ![image-20210127160540536](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210127160540536.png)

  flex-flow :复合属性,相当于同时设置了flex-direction和flex-wrap

  ![image-20210127164500659](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210127164500659.png)

+ 子项常见属性

  flex 子项目占的份数

  ![image-20210127171826996](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210127171826996.png)

  align-self  控制子项自己在侧轴的排列方式order属性定义子项的排列顺序(前后顺序)
  
  ![image-20210127200002405](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210127200002405.png)
  
  order
  
  ![image-20210127200328205](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210127200328205.png)

**携程实战**

背景线性渐变   ==背景渐变必须添加浏览器的私有前缀==

![image-20210202100831762](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210202100831762.png)

![image-20210202101313212](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210202101313212.png)

## rem基础

em 单位

![image-20210209154240684](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210209154240684.png)

rem 单位

![image-20210209154404697](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210209154404697.png)

## 媒体查询

媒体查询(Media Query ）是CSS3新语法。
使用@media查询，可以针对不同的媒体类型定义不同的样式

**@media可以针对不同的屏幕尺寸设置不同的样式**

当你重置浏览器大小的过程中，页面也会根据浏览器的宽度和高度重新渲染页面

目前针对很多苹果手机、Android手机，平板等设备都用得到多媒体查询

![image-20210221160544542](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210221160544542.png)

![image-20210221161018931](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210221161018931.png)

![image-20210221161156449](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210221161156449.png)

![image-20210221163130437](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210221163130437.png) 

![image-20210221163225498](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210221163225498.png)

最好是**从小到大**写，这样可以利用**层叠性**覆盖前面写的

## 媒体查询+rem实现元素动态大小变化

rem单位是跟着html来走的，有了rem页面元素可以设置不同大小尺寸媒体查询可以根据不同设备宽度来修改样式

媒体查询+rem 就可以实现不同设备宽度，实现页面元素大小的动态变化

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  <style>
    @media screen and (min-width: 320px) {
      html {
        font-size: 50px;
      }
    }

    @media screen and (min-width: 640px) {
      html {
        font-size: 100px;
      }
    }

    .top {
      height: 1rem;
      font-size: .5rem;
      background-color: #bfa;
      color: #fff;
      text-align: center;
      line-height: 1rem;
    }
  </style>
</head>
<body>
  <div class="top">购物车</div>
</body>
</html>
```

**引入资源**

当样式比较繁多的时候，我们可以针对不同的媒体使用不同stylesheets(样式表)。原理，就是直接在link中判断设备的尺寸，然后引用不同的css文件。

![image-20210221181657492](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210221181657492.png)

![image-20210221182651734](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210221182651734.png)

## Less基础

![image-20210221190027169](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210221190027169.png)

![image-20210222161748589](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210222161748589.png)

Less使用
我们首先新建一个后缀名为less的文件，在这个less文件里面书写less语句。

**Less变量**

![image-20210222161957359](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210222161957359.png)

1.变量命名规范

+ 必须有@为前缀
+ 不能包含特殊字符
+ 不能以数字开头大小写敏感

**Less编译**

​    本质上，Less包含一套自定义的语法及一个解析器，用户根据这些语法定义自己的样式规则，这些规则最终会通过解析器，编译生成对应的CSS文件。
​    所以，我们需要把我们的less文件，编译生成为css文件，这样我们的html页面才能使用。

+ vscode Less插件

![image-20210222193033893](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210222193033893.png)

**Less嵌套**

![image-20210223182321679](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210223182321679.png)

![image-20210223183050882](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210223183050882.png)

（交集 应该是指 并集）

**Less运算**

![image-20210223192046467](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210223192046467.png)

1. 我们运算符的左右两侧必须敲一个空格隔开   1px + 5
2. 两个数参与运算如果只有一个数有单位，则最后的结果就以这个单位为准
3. 两个数参与运算，如果2个数都有单位，而且不一样的单位最后的结果以第一个单位为准

## rem适配方案

![image-20210223194935209](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210223194935209.png)

## less中导入less文件

![image-20210225145650087](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210225145650087.png)

+ @import导入的意思可以把一个样式文件导入到另外一个样式文件里面

+ link是把一个样式文件引入到 htm1页面里面

**flexible.js**

![image-20210228172854772](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210228172854772.png)

https://github.com/amfe/lib-flexible

flexible.js 给我们划分了 **10** 等分，只需要将网址中的 Js 文件引入即可实现 html 的 font-size 随窗口的大小而等比例缩放，从而使用 rem 适配方案，因此相对于方案一来说不需要 less 文件。

**vscode 插件 px 转换 rem  插件 cssrem**

这个插件默认的 html 文字的大小 cssroot : 16px，需要根据设计稿的大小修改默认文字的大小

+ 修改方法：在 vscode 的设置中搜索 setting.json 文件，修改"cssrem.rootFontSize":16 的值即可 

## 响应式布局

就是使用**媒体查询**针对不同宽度的设备进行布局和样式的设置，从而适配不同设备的目的。

![image-20210307212637807](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210307212637807.png)

![image-20210307212929249](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210307212929249.png)

图片上通过媒体查询来实现

![image-20210307213437058](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210307213437058.png)

### Bootstrap前端开发框架

中文官网: http://www.bootcss.com/

官网: http://getbootstrap.com/
推荐使用: http://bootstrap.css88.com/

![image-20210307214930524](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210307214930524.png)

bootstrap 里面已经包含了 normalize.css ，无需再次引入

![image-20210307215213198](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210307215213198.png)

![image-20210307215602027](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210307215602027.png)

![image-20210307215827503](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210307215827503.png)

### Bootstrap栅格系统

![image-20210307220511079](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210307220511079.png)

![image-20210308091713346](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210308091713346.png)

**注意**：需要下载bootstrap才能实现

![image-20210308092602170](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210308092602170.png)

![image-20210308094624267](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210308094624267.png)

![image-20210308094516484](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210308094516484.png)

![image-20210308095606960](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210308095606960.png)

push 是从左向右推， pull 是从右向左拉

![image-20210308100043735](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210308100043735.png)

## 移动端总结

![image-20210308130210157](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210308130210157.png)

![image-20210308130235462](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210308130235462.png)

建议︰我们选取一种主要技术选型，其他技术做为辅助，这种混合技术开发

# swiper实现位移动画

用来实现位移动画 

官网：https://www.swiper.com.cn/

官网上有文档说明

# git

![image-20210307203951567](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210307203951567.png)

![image-20210307204119652](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210307204119652.png)

![image-20210307204514628](D:\学习文件\笔记OLY\html css\html-css.assets\image-20210307204514628.png)

 