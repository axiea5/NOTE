### Html和CSS 第一天

#### 常用浏览器

IE、火狐浏览器、谷歌浏览器、Edge浏览器、Safari浏览器、Opera浏览器

#### 浏览器内核

(1)Trident（IE内核）
(2)Gecko（firefox）
(3)Webkit（safari）
(4)Chromium/Blink（chrome）

#### Web标准构成

结构（structure）、表现（presentation）、行为（behavior）

#### Html

超文本标记语言 

#### Html骨架

Html标签
head标签：文档的头部
title标签：文档的标题
body标签：文档的主体

#### 标签关系

1. 嵌套关系
2. 并列关系

#### Html常用标签

标题：<h1><h2><h3><h4><h5><h6>
段落：<p>
水平线标签：<hr/>
换行标签：<br/>

#### 文本格式化标签

粗体：<b></b>  <strong></strong>
斜体：<i></i>  <em></em>
加删除线：<s></s>  <del></del>
加下划线：<u></u>  <ins></ins>

#### 图像标签

单标签

```
<img src=”图片路径” alt=”无图片显示文字” title=”鼠标放在图片上显示文字” height=”高” weight=”宽” border=”边框”>
```

链接标签

```
<a href=”跳转目标” target[ Target取值：self：默认值、_blank：新窗口中打开]=”目标窗口的弹出方式”>文本或图像<a>
```

#### 锚点定位

(1)

```
<a href="#id">链接</a>
```

(2)

```
<P id="id"></p>
```



#### Base标签

可以设置整体连接的打开状态
Head里 

```
<base target=”_blank”/>
```

#### 注释标签

```
<!--注释-->
```

#### 路径

##### 相对路径：

（1）图像文件和html文件位于同一文件夹中：<img src=”1.jpg”>
（2）图像文件位于html文件的下一级文件夹：<img src=”img/1.jpg”>
（3）图像文件位于html文件的上一级文件夹：<img src=../1.jpg>

##### 绝对路径：

（1）<img src=”C:\Users\apple\1.jpg”>
（2）网络图片地址

#### 列表标签

##### 无序列表ul：前面带小黑圆点

```
<ul>
<li></li>
</ul>
```

##### 有序列表ol：1.2.3.排列

##### 自定义列表

```
<dl>
<dt>名词</dt>
<dd>名词解释1</dd>
<dd>名词解释2</dd>
</dl>
```



### Html和CSS 第二天

#### 表格table

```
<table width=”500” border=”1”>
<tr>行
<td></td>列
</tr>
</table>
```

#### 表格属性

Align：水平对齐方式：left、center、right
Cellspacing：设置单元格与单元格边框之间的空白间距
Cellpadding：设置单元格内容与单元格边框之间的空白间距
Border：边框

#### 表头标签<th></th>

加粗居中，第一行或第一列

#### 表格标题caption

Table标签之后，居中
每个表格只能定义一个标题

#### 表格结构

头部<thead></thead>
主体<tbody></tbody>

#### 合并单元格

跨行合并rowspan：竖
跨列合并colspan：横
从上而下、自左而右

#### Label标签

```
<label for="pwd">
用户名：<input type="text">
密码：<input type="password" id="pwd"><>
</label>
```

点击文字光标定位到该文本框

#### Textarea文本域

```
<textarea col=”每行字符” rows=”行数”><textarea>
```

#### 下拉菜单select

```
<select>
<option selected=”selected”[ selected=”selected”：被选中]></option>选项
</select>
```

#### Input标签

1. Type属性
   Text：单行文本输入框
   Password：密码输入框
   Radio：单选按钮
   Checkbox：复选框
   Button：按钮
   Submit：提交按钮
   Reset：重置按钮
   Image：图像形式的提交按钮
   File：文件域
2. Name：名称，一组中只有一个
3. Value：默认文本
4. Size：显示宽度
5. Checked：默认被选中的项
6. Maxlength：允许输入最大字符数

#### 表单域

```
<form action=”url地址” method[ Method取值为get或post]=”提交方式” name=”表单名称”></method>
```

#### 内部样式表

```
<head>
<style type=”text/css”>
选择器{属性1：属性1；属性2：属性2；属性3：属性3；}
</style>
</head>
```

#### 行内式（内联样式）

```
<标签名 style=”属性1：属性1；属性2：属性2；属性3：属性3；”>内容</标签名>
```

#### 外部样式表（外链式）

```
<head>
<link href=”css文件路径” type=”text/css” rel=”stylesheet”/>
</head>
```

#### 标签选择器（元素选择器）

标签{属性1：属性1；}

#### 类选择器

.类名{属性1：属性1；}
Body内标签调用加class=”类名”
多类名选择器类名之间用空格隔开



### Html和CSS 第三天

#### 类选择器与id选择器的区别

类选择器可以多次重复使用
Id选择器是唯一的，不能重复

#### 通配符选择器

```
*{属性1：属性1；}
```


匹配页面所有元素

#### Font-family：字体

- 尽量使用偶数数字字号
- 字体之间用逗号隔开
- 字体名包含空格和符号时需加引号
- 尽量使用默认字体

#### Font-weight：字体粗细（strong b）

Normal（正常400）、bold（粗体700）、Bolder（特粗）、lighter（细体）、100-900（100的整数倍）

#### Font-style：字体风格（不常用）（em i）

Normal、italic（斜体）、oblique（倾斜）

#### 字体连写（不能更换顺序）

选择器{font：font-style font-weight font-size/line-height font-family[ 必须保留font-size和font-family]；}

#### Text-align：水平对齐方式

Left、right、center

#### Text-indent：首行缩进

1em一个字宽度

#### Text-decoration：装饰（ins u）

None（取消装饰）、underline

#### 后代选择器

```
.父 子{属性：值}
```

中间空格隔开
所有后代

#### 子代选择器

```
.父>子{属性：值}
```

'>'隔开
直属子代，最好不超过3个

#### 交集选择器（不常用）

既又关系

```
P.one{属性：值}
```

#### 并集选择器

逗号隔开

```
标签，标签{属性：值}
```

#### 链接伪类选择器

：link  未访问的链接
：visited  已访问的链接
：hover  鼠标移动到连接上
：active  鼠标点击时候
注意写的时候顺序不要颠倒lv hao

#### 快捷方式

兄弟关系标签+
带有类名和id名.demo或#two 然后tab（div）
Input：加type内容 然后tab（直接tab是text）

#### 块级元素

独占一整行或多行，
可以设置宽高、对齐、内、外边距属性
宽度默认是容器的100%
可以容纳内联元素和其他块元素
H1~h6、p、div、ul、ol、li

#### 行内元素（可以看做文字text-align）

和相邻行内元素在一行上
宽高无效、可以设置水平的padding和margin
宽度默认是本身内容宽度
行内元素只能容纳文本或其他行内元素（a里面可以放块级元素）
P、h1这类里面不能放块级元素，链接里面不能放链接
A、strong、b、em、i、del、s、ins、u、span

#### 行内块元素（可以看做文字text-align）

和相邻行内元素（行内块）在一行，之间会有空白间隙
默认宽度就是他本身内容的宽度
宽高、内外边距可以控制
Img、input、td

#### 标签显示模式转换display

块转行内：display：inline
行内转块：display：block
块、行内、转行内块：display：inline-block

行内、行内块元素可以看做文本，居中对齐text-align

行高等于盒子高度，可以让文本垂直居中line-height=height

### Html和CSS 第四天

#### 行高

顶线、中线、基线、底线
行高=基线与基线的距离
文字垂直居中=行高等于高度 

#### 权重

- *或继承       0.0.0.0     *
- 元素（标签）  0.0.0.1     p
- 类，伪类      0.0.1.0     .
- Id             0.1.0.0    #
- 行内样式      1.0.0.0    元素后直接使用
- ！Important    +∞
  权重相同，就近原则
  权重会叠加，没有进制

##### 从小到大排列：

*或继承<标签<类，伪类<id<行内<！important

#### 背景background

Background：transparent透明 url（image.jpg）图片 repeat-y平铺 scroll滚动 50% 0 无强制标准

##### (1)Repeat平铺

No-repeat:不平铺
Repeat-x：横向平铺
Repeat-y：纵向平铺

##### (2)Position

Length：百分数
Position：top、center、buttom、left、right
xpx ypx横纵定位
没有上下顺序
只有一个值，另一个默认居中
可以用px，先x后y

##### (3)Attachment

Scroll：背景图像随内容滚动（默认）
Fixed：背景图像固定

##### (4)Color

##### (5)Image

#### 背景透明CSS3

Background：rgba（0,0,0,0.3）
Rgba：red green blue alpha0-1

#### 盒子模型

##### （1）盒子边框border

Width、style、color
Table{border-collapse：collapse；}合并相邻边框

##### （2）内边距padding

顺时针
有宽高时会撑开盒子

##### （3）外边距margin

#### 背景图百分比

背景图的百分比不是按照容器的大小去换算的
百分比的背景定位：容器的宽度（高度）-背景的宽度（高度）*百分比
background:url(“ ”)no-repeat 25% bottom/1200px 800px

### Html和CSS 第五天

#### 盒子水平居中

Margin：0 auto 上下0左右auto
Margin-right：auto左上角，自动充满右边

**必须块级元素**

**盒子必须有宽度**

#### 相邻外边距合并

两个相邻元素外边距以大的为准

#### 嵌套块元素垂直外边距的合并（外边距塌陷）

父元素上外边距=0，
则父元素的上内边距会与子元素的上外边距发生合并，合并后以较大的为准
(1)父元素上边框或上内边距
(2)父元素添加overflow：hidden

#### 根据稳定性

Width>padding>margin

#### 盒子圆角CSS3

```
Border-radius:50%（圆，上限）
Border-radius：1px 1px 1px 1px 上左右下右左（顺时针）
```


越大越圆

#### 盒子阴影

```
Box-shadow：h-shadow水平阴影 v-shadow垂直阴影 blur模糊距离 spread阴影尺寸 color阴影颜色（rgba） inset内/外阴影
```


前两个必写，默认外阴影（outset），内阴影inset

#### 浮动

Left、right、none（默认）
脱离标准流（脱标），不占位置，影响标准流
不会超过内边距
与父级元素搭配使用
可以让元素默认转换为行内块元素

#### 版心

网页主体内容所在区域，居中显示
960px、980px、1000px、1200px

#### Ps基本使用

Ctrl+r 显示隐藏标尺。右击标尺，改为像素
Alt+鼠标滚轮上下滑动 放大缩小
Shift+鼠标滚轮上下滚动 图片上下移动
Ctrl+d 取消选区

#### 切片

导出切片：文件-存储为web设备所用格式



### Html和CSS 第六天

#### 清浮动

解决父级元素因为子级浮动引起内部高度为0的问题
不是所有浮动都需要清除，影响布局才需要清除

```
选择器{clear：属性值；}
属性值：Left、right、both
```

#### 额外标签法（w3c推荐）

**浮动元素末尾**添加一个空标签

```
<div style=”clear:both”></div>或其他标签br等
<div class=”clear”><div>
.clear{clear:both}
优点：通俗易懂，书写方便
缺点：添加许多无意义的标签，结构优化较差（不好）
```

#### 父级添加overflow属性方法（触发BFC）

给**父级元素**添加

```
Overflow：hidden/auto/scroll
优点：代码简洁
缺点：内容增多时候容易造成不会自动换行导致内容被隐藏掉，无法显示需要溢出的元素
```

#### 使用after伪元素

空元素升级版，不用单独加标签

```
.clearfix:after{
content:””;
display:block;
height:0;
clear:both;
visibility:hidden;}
.clearfix{*zoom:1}  （IE7专有） 
优点：符合闭合浮动思想 结构语义化正确
缺点：由于IE6-7不支持：after，使用zoom：1触发hasLayout
```

visibility:hidden：指定一个元素不可见
百度、淘宝、网易

#### 双伪元素（before、after）

```
.clearfix:before,.clearfix:after{
content:””;
display:table; (这句话可以触发BFC清除浮动)}
.clearfix:after{
Clear:both;}
.clearfix{
*zoom:1;
}
优点：代码更简洁
缺点：由于IE6-7不支持：after，使用zoom:1触发hasLayout
```


小米

#### 定位（position）

1. ##### 边偏移

   top、bottom、left、right

2. ##### 定位模式（分类）子绝父相 脱标

   **Static 自动定位（默认）**
   **Relative 相对定位**
   相对于原位置。以自己左上角为基点，原来所占位置继续占有
   **Absolute 绝对定位**
   相对于上一个已经定位的父元素（父元素没定位就以当前屏幕为准），类似浮动
   **Fixed 固定定位（电梯导航）**
   相对于浏览器窗口

#### 绝对定位的盒子居中对齐

加了定位和浮动， margin：0 auto会失效

```
（1）left：50% 走到父盒子一半
（2）margin-left：负一半外边距（盒子一半值）
```

#### 绝对定位和固定定位模式转换

```
Width:100%
Top:0
Left:0
```

#### 叠放次序（z-index）

1. 默认:  0，取值越大越靠上
2. 取值相同:根据书写顺序，后来的靠上
3. 后面数字不能加单位
4. 只有相对定位、绝对定位、固定定位有这个属性

### Html和CSS 第七天

#### 显示与隐藏

1. Display:none/block 隐藏/显示某个元素
   隐藏后**不保留位置**
2. Visibilit：visible/hidden 对象可见/隐藏
   隐藏后**保留位置**
3. overflow：hidden/scroll/auto 显示超过对象尺寸的内容/总是显示滚动条/在需要时剪切内容并添加滚动条

#### 鼠标样式cursor

```
Default：默认
Pointer：小手
Move：移动
Text：文本
```

#### 轮廓线outline

None/0：取消轮廓线（蓝色边框）
主要是input里面

#### 防止拖拽文本域（textarea）resize

None：防止火狐、谷歌等浏览器随意拖动文本域

#### 垂直对齐vertical-align（图片与文字对齐）

- Baseline：默认（基线对齐）

- Top：顶部对齐

- Middle：垂直居中

- Bottom：底部
  与行内块元素搭配使用，不影响块级元素中的内容对齐，只针对行内或行内块，特别是行内块
  图片或表单等行内块元素，底线会和父级元素基线对齐，造成图片底侧有空白缝隙

  解决：
  （1）给img vertical-align：middle/top。。，让图片不要和基线对齐
  （2）给图片转换成块级元素：display：block

#### 溢出文字隐藏（根据浏览器默认显示不一样 ）

White-space：nowrap 强制在同一行内显示所有文本，知道文本结束或遇到br
Text-overflow：clip/ellipsis 直接裁切/溢出部分...标记
需要先强制一行内显示，然后和overflow搭配使用

#### CSS精灵技术（sprite）小妖精 雪碧

主要作为背景图像
有效减少服务器接受和发送请求的次数，提高页面加载速度
使用fw测量，软件内用打开图，记得上锁
Background-position精确定位(基本都是负的)

#### 滑动门

原因：字数不一样，不适合写宽

```
<li><a><span></span></a></li>
```

A的background是放左边的圆角
Span放右边圆角 
最好左右加padding值

#### 图片上鼠标滑过播放按钮

```
Width:100%;
Height:100%;
Background:rgba(0,0,0,.5) url() center no-repeat
```

### Html和CSS 第八天

#### 字体图标

本质是文字，可以改颜色，阴影，透明效果
也可以做图片一样的事情
体积小，携带信息无缩减
几乎支持所有浏览器

**1.解压-->Fonts文件加入文件夹-->style声明字体引入**

```
@font-face {  /*声明字体  引用字体*/
	font-family: "icomoon";  /*我们可以自己起名字*/
	src:url('fonts/icomoon.eot?7kkyc2');
	src:url('fonts/icomoon.eot?7kkyc2#iefix')format('embedded-opentype'),
	url('fonts/icomoon.ttf?7kkyc2') format('truetype'),
	url('fonts/icomoon.woff?7kkyc2') format('woff'),
	url('fonts/icomoon.svg?7kkyc2#icomoon') format('svg');
	font-style: normal;  /*倾斜字体正常*/}
元素span {font-family:”icomoon”;}
```

**2.Body里直接复制粘字体解压后文件demo.html里选中图标后面小方块**
前面是伪类元素用的

```
Span：：before{content：”\e900”；}
```

#### Svg转字体图标

Icomoon里左上角inport icons

#### 追加字体图标

无法合并
点击Import icons导入以前压缩后文件里的selection.json

#### 行高1.5

字体大小*1.5
不用设置高度 

#### 网页ico

放根目录
网址后加favicon.Ico

```
<link rel=”shortcut icon” href=”favicon.ico” />
```

#### logo制作

```
<Div class=”logo”>
<h1>
<a href=”#”>京东</a>
</h1>
```

#### 网站说明description

- 关键词要详细，是给别人看的
- 含空格在内不要超过120个汉字
- 是title和keywords的补充说明
- 中间最好用英文

```
<meta name=”description” content=”哒哒哒”/>
```

#### 关键字keywords

6~8个关键词

```
<meta name=”keywords” content=”小米，大米”/>
```



### Html和CSS 第十天

**Ie9以上**

#### 新增表单input

```
Email：请在电子邮件地址中包括“@”
Tel：
Url：请输入网址
Number：右边有上下箭头︿﹀，可以增加减少。只能输入数字键
Range：拖动滑块，根据浏览器不一样
Time: --:-- ︿﹀
Date: 年 /月/日 ︿﹀，有下拉选框
Datetime：
Month；月份 ----年--月
Week：周  ----年第--周
```

#### 新增属性

```
Placeholder：相当于value，光标定进去输入字才消失
Autofocus：页面加载完毕，光标自动获取定位到里面
Multiple：多文件上传
Autocomplete：表单启动自动完成功能
Required：必填项 内容不能为空
Accesskey：规定激活（使元素获得焦点）元素的快捷键
```

#### 插入视频

Audio：音频（ogg、mp3、wav）
(1)**autoplay**：自动播放
(2)**Controls**：是否显示不默认播放控件
(3)**Loop**：循环播放

#### Css3新增选择器

结构（位置）伪类选择器
**：first-child**
**：last-child**
**：nth-child（n）** 匹配属于其父元素的第N个子元素，不论元素的类型
**：nth-last-child（n**） 选择器匹配属于其元素的第N个子元素的每个元素，不论元素类型，从后往前，n可以是数字、关键词或公式
  **Even**（偶数）、**odd**（奇数）

#### 属性选择器

```
Attribute[ ]{}
div[class]{background-color:pink;} 

div[class=demo]{background-color:pink;}
 class=demo

div[class^=demo]{background-color:pink;}  
 class名开头是demo

div[class$=demo]{background-color:pink;} 
 class名末尾是demo
```

#### 伪元素

```
：：first-letter{} 第一行
：：first-line{} 第一个字
：：selection{} 选中文本
：：before{content：“”；} 
内部插入，必须写content 相当于一个盒子
```

#### Css3盒子模型

**box-sizing：**
border-box内减模式，包含margin、padding，会自动调整
Content-box以前的

### Html和CSS 第十一天

#### 过渡Transition

**Transition**：要过渡的属性 花费时间 运动曲线 何时开始；  多组变化，用逗号隔开

**Transition-property**：属性名称  全部用all

**Transition-duration**：花费时间。默认0

**Transition-timing-function**：时间曲线。Linear匀速、ease逐渐慢下来（默认）、ease-in加速、ease-out减速

**Transition-delay**：何时开始。默认0
过渡写到本身上，谁做过渡动画，写到谁身上

#### 2d变形Transform

**translate(x,y)**   移动（只有x  y默认为0）

**scale(x,y)**      缩放（取值0-1）
（只有x  y默认等比例缩放）

**Rotate（deg）**  旋转

**skew(deg，deg)** 倾斜

**Transform-origin**：可以调整元素转换变形的原点

**transform**: translate(-50%,-50%); 定位走盒子一半
顺序有关系，先前

### Html和CSS 第十二天

#### 动画（css3）animation

**Animation**：动画名称 动画时间 运动曲线 何时开始 播放次数（无限次播放：infinite） 是否反方向（轮流反向播放：alternate）完成状态（保持当前：forwards 回到起点：backwards）

```
声明动画：@keyframes 动画名称{ 
from：{ } 
To{ }
}
```

#### 伸缩布局flex

```
父元素 display：flex；
子元素 flex：1（份数）
min-width：最小宽度
Flex-direction：column/row
```


调整主轴方向：垂直/水平(默认)

#### 文字阴影（css3）

**Text-shadow**：水平位置 垂直位置 模糊距离 阴影颜色；

#### 背景缩放（css3）background-size

（1）可以设置长度单位（px）或百分比（设置百分比时，参照盒子的宽高）

（2）cover，会自动调整缩放比例，保证图片始终填充满背景区域，溢出会隐藏

（3）Contain，会自动调整缩放比例，保证图片始终完整显示在背景区域

#### 浏览器前缀

```
-webkit-  google chrome、safari，Android browser
-moz-  firefox
-o-  opera
-ms-  Internet explorer、edge
-khtml-  konqueror
```

#### 背景渐变(兼容性差)

Backround：-webkit-linear-gradient（渐变的起始位置，起始颜色，结束颜色）
Backround：linear-gradient（渐变的起始位置，颜色 位置，颜色 位置...）

#### 多背景

中间空格隔开，颜色写到下面，防止被叠加

#### 优雅降级和渐进增强

**渐进增强progressive enhancement**
针对低版本浏览器进行构建页面，保证最基本的功能，然后在针对高级浏览器进行效果、交互等试验
**优雅降级graceful degradation**
一开始就构建完整的功能，然后在针对低版本浏览器进行兼容

#### 3D变形（css3）transform

**RotateX**（）、**RotateY**（）、**RotateY**（）

#### 透视（perspective）

**Backface-visibility**当元素不面向屏幕时是否可见

#### js实现动画，css显示动画（区别）

一个是帧动画（js），一个是补间动画（css）
帧动画：使用定时器，每隔一段时间 更改当前元素的状态
补间动画：过渡（加过渡，只要状态发生改变） 动画（多个节点来控制动画）性能更好
在支持H5C3的浏览器尽可能使用css3动画（尤其是移动端开发）

#### 转换

缩放：**scale**
位移：**translate**
旋转：**rotate**
倾斜：**skew**
以上四种转换方式是比较特殊，其实他们都是由matrix矩阵

#### 动画速度

**ease**：先快后慢 最后非常慢
**linear** 匀速
**ease-in** 速度越来越快
**ease-out** 速度越来越慢
**ease-in-out** 速度先快后慢
以上五种动画速度比较特殊，其实他们是由贝塞尔曲线来的

#### 2d转换和3d转换区别

1. 除了多了一个参数表示3d
2. 在移动端使用3d转换可以优化性能（如果设备有3d加速引擎 GPU可以提高性能， 2d转换无法调用GPU）

### 笔记

#### 元素转换

(1)display:inline;转换为行内元素
(2)display:block;转换为块状元素
(3)display:inline-block;转换为行内块状元素

#### 清浮动

可以设置高度或者清浮动

#### display: inline-block;布局会造成两个问题：

1. **两个div没有对齐。** 
   **原因**：（1）同一行的行内元素对齐方式默认是基线对齐，即vertical-align：baseline
   （2）对于内容为空的inline-block元素而言，该元素的基线就是它的margin底边缘，否则就是元素的内部最后一行内联元素的基线
   **解决**：为inline-block元素添加vertical-align: top
   vertical-align：设置元素的垂直对齐方式
2. **两个div之间会有一个间隙**
   **原因**：inline-block会引起元素和元素之间几个像素的间隙（具体间隙大小取决于字体大小）。造成空白间隙的原因是在标签和标签之间使用了空格或换行符。因为空白字符也是字符，也会引用CSS样式。
   **解决**：设置父元素的font-size为0，在子元素重新设置字体大小。

#### Background-size背景尺寸

**Length：xpx ypx**（如果只有一个值，第二个则是auto）
**Percentage**：相对于背景定位区域的百分比。X% y%（如果只有一个值，第二个则是auto）
**Cover**：保持横纵比将图像缩放成完全覆盖背景定位区域的最小大小
**Contain**：保持横纵比将图像缩放成适合背景定位区域的最大大小

#### 图片居中

**vertical-align: middle;**
旁边没有文字需要加一个空白span

#### Div内图片居中

**在不清楚图片图片或元素的真实宽高情况下：（position）**

```
Div：position: relative;
    width: 185px;
    height: 60px;
    overflow:hidden;
Img： position: absolute;
    max-width: 100%;
    height: auto;
    top: 50%;
    left: 50%;
transform: translate3d(-50%,-50%,0);
```

#### 3种解决子元素margin带动父元素移动

1. ```
   overflow: hidden;
   ```

2. 给父元素加边框

   ```
   border: 1px solid #000000;
   ```

3. 父元素内边距，与子元素保持距离

   ```
   padding-top: 1px;
   box-sizing: border-box;//保持尺寸，因为如果指定height的话，padding-top会增加高度
   ```

#### li:hover使li中a标签颜色改变

a元素继承的权重没有a标签浏览器默认设置的高

```
ul li:hover a{ color: #ffa000;}
```

#### padding撑大盒子解决办法

```
box-sizing: border-box;
```

#### -webkit-line-clamp超过两行就出现省略号

```
overflow : hidden;
text-overflow: ellipsis;
display: -webkit-box; 必须结合的属性 ，将对象作为弹性伸缩盒子模型显示 。
-webkit-line-clamp: 2;
-webkit-box-orient: vertical; 必须结合的属性 ，设置或检索伸缩盒对象的子元素的排列方式 。
```

#### word-break 属性

break-all	允许在单词内换行。
keep-all 只能在半角空格或连字符处换行。 

#### 改变hr颜色

```
hr{
background-color:blue;
Border:none;
Height:1px;
Margin:0;
}
```

#### 伪元素选择器

::after
::before
::first-letter
::first-line
::selecton

#### 边框图片 border-image

由于浏览器兼容问题，没有广泛使用，了解即可**
在内容变化的容器可以使用，边框自动填充
**属性：**
1.**图片链接**: border-image-source
url(“ ”)

2.**切割的尺寸**:border-image-slice
默认单位是px 不能使用小数
   切割的位置距离对应的边的距离 切了四刀 4个切割尺寸

3.**边框的宽度** border-image-with

4.**平铺的方式** border-image-repeat
    3种方式：**round**环绕（完整的自适应平铺在边框内） 
                      **stretch** 拉伸（拉伸显示在边框内容 变形的） 
                      **repeat**平铺（从边框的中间向两侧平铺 自适应平铺但是不是完整的）
border-image:url(“ ”) 167/20px round;

#### 语义化标签的作用

1. 从开发角度考虑是提高代码的可读性、可维护性
2. 网站发布者：seo搜索引擎优化

#### 语义化标签的兼容问题

1. IE9以下不支持H5标签（大部分css3属性，一些H5的api）
2. IE9一下不认识，把这些标签当做行内元素去看待
3. 语义化标签需要动态创建 document.createElement(‘header’) 同时设置块级元素
4. 利用插件完成事件 html5shiv.js