## css 语法结构
---------------------------

![css语法结构图](./img/css-struct.png)

## 选择器
--------------------------

- 标签选择器

```css
  div {line-height: 30px}
```

- ID 选择器

```css
  #main-wrapper {width: 500px; margin: 10px auto;}
```

- class 选取器

```css
  .clear {clear: both;}
```

- 组合选择器

```css
  #wrapper li {list-style: none; width: 150px;}
```

> 更多子类选择器；相邻选择器；属性选择器；伪类选择器参考w3c文档

## css 盒模型
---------------------------
![css盒模型图](./img/css-box.png)

大小： width, height

边框： border

内边距:  padding

外边距:  margin

-   边框和内边距及外边距都会占用元素布局空间；因此计算时要考虑这些因素
-   外边距可以使用负值；但是其它属性不可以；
-   各属性都可以单独定义四边大小； 
-   单行定义（(上下-左右；顺时针方向 分别为top – right-bottom-left)）
-   只有块元素设置`width` 、 `height`属性有效

> 上下外边距自动合并, 参考w3c文档


## 显示方式 display

隐藏元素： display: none

- 区别 `visibility: hidden`

显示为块元素: `display: block`

显示为内联元素: `display: inline`

<table class="dataintable">
<tbody><tr>
<th>值</th>
<th>描述</th>
</tr>
<tr>
<td>none</td>
<td>此元素不会被显示。</td>
</tr>

<tr>
<td>block</td>
<td>此元素将显示为块级元素，此元素前后会带有换行符。</td>
</tr>

<tr>
<td>inline</td>
<td>默认。此元素会被显示为内联元素，元素前后没有换行符。</td>
</tr>

<tr>
<td>inline-block</td>
<td>行内块元素。（CSS2.1 新增的值）</td>
</tr>

<tr>
<td>list-item</td>
<td>此元素会作为列表显示。</td>
</tr>

<tr>
<td>run-in</td>
<td>此元素会根据上下文作为块级元素或内联元素显示。</td>
</tr>
<tr>
<td>table</td>
<td>此元素会作为块级表格来显示（类似 &lt;table&gt;），表格前后带有换行符。</td>
</tr>

<tr>
<td>inline-table</td>
<td>此元素会作为内联表格来显示（类似 &lt;table&gt;），表格前后没有换行符。</td>
</tr>
<tr>
<td>inherit</td>
<td>规定应该从父元素继承 display 属性的值。</td>
</tr>
</tbody>
</table>



## 定位: position
---------------------------

通过使用 `position` 属性，我们可以选择 4 种不同类型的定位，这会影响元素框生成的方式。

- static

元素框正常生成。块级元素生成一个矩形框，作为文档流的一部分，行内元素则会创建一个或多个行框，置于其父元素中。

- relative

元素框偏移某个距离。元素仍保持其未定位前的形状，它原本所占的空间仍保留。

- absolute

元素框从文档流完全删除，并相对于其包含块定位。包含块可能是文档中的另一个元素或者是初始包含块。元素原先在正常文档流中所占的空间会关闭，就好像元素原来不存在一样。元素定位后生成一个块级框，而不论原来它在正常流中生成何种类型的框。

- fixed

元素框的表现类似于将 position 设置为 absolute，不过其包含块是视窗本身。

> position 属性说明定位方式；位置确定可以通过属性`top` `right` `bottom` `left`实现

```css
  {
      position:absolute;
      left:100px;
      top:150px
  }
```

## 浮动: float
-------------------------

> 浮动的框可以向左或向右移动，直到它的外边缘碰到包含框或另一个浮动框的边框为止。

![左浮动](./img/float-left.gif)

![右浮动](./img/float-right.gif)

> 浮动元素脱离原默认的布局空间；如果要占用一定空间，不遮住其它元素，需要用到`clear`属性

> 

## 样式

- 背景

--  背景颜色 `background-color`

--  背景图片 `background-image`

--  背景重复 `background-repeat`

--  背景位置 `background-position`


```css
    p {background-color: gray;}
    body { 
        background-image: url("/i/eg_bg_03.gif");
        background-repeat: no-repeat;
        background-position: -60px -30px;
    }
```


- 文本

<table>
<tbody>
<tr>
  <th>属性</th>
  <th>描述</th>
</tr>
<tr>
<td>color</td><td>设置文本颜色</td>
</tr>
<tr>
  <td>line-height</td><td>设置行高。</td>
</tr>
<tr>
  <td>letter-spacing></td><td>设置字符间距。</td>
</tr>
<tr>
  <td>text-align</td><td>对齐元素中的文本。</td>
</tr>
<tr>
  <td>text-decoration</td><td>向文本添加修饰。</td>
</tr>
<tr>
  <td>text-indent</td><td>缩进元素中文本的首行。</td>
</tr>
<tr>
  <td>text-shadow</td><td>设置文本阴影。CSS2 包含该属性，但是 CSS2.1 没有保留该属性。</td>
</tr>
<tr>
  <td>word-spacing</td><td>设置字间距。</td>
</tr>
</tbody>
</table>



- 链接

```css
  a:link {text-decoration: none;}
  a:visited {text-decoration: none;}
  a:hover {text-decoration: underline;}
  a:active {text-decoration: underline;}
```

- 列表

<table>
  <tbody><tr>
    <th>属性</th>
    <th>描述</th>
  </tr>
  <tr>
    <td>list-style</td>
    <td>简写属性。用于把所有用于列表的属性设置于一个声明中。</td>
  </tr>
  <tr>
    <td>list-style-image</td>
    <td>将图象设置为列表项标志。</td>
  </tr>
  <tr>
    <td>list-style-position</td>
    <td>设置列表中列表项标志的位置。</td>
  </tr>
  <tr>
    <td>list-style-type</td>
    <td>设置列表项标志的类型。</td>
  </tr>
  
</tbody></table>


## 嵌入样式方法
-------------------------

###外部样式表

```html
    <head>
    <link rel="stylesheet" type="text/css" href="mystyle.css" />
    </head>
```

### 内部样式表

```html
    <head>
    <style type="text/css">
      hr {color: sienna;}
      p {margin-left: 20px;}
      body {background-image: url("images/back40.gif");}
    </style>
    </head>
```
### 内联样式

```html
<p style="color: sienna; margin-left: 20px"></p>
```


