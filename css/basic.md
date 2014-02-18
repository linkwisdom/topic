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

## 样式

- 背景

-- 背景颜色 `background-color`
-- 背景图片 `background-image`
-- 背景重复 `background-repeat`
-- 背景位置 `background-position`

``css
  p {background-color: gray;}

  body { 
      background-image: url('/i/eg_bg_03.gif');
      background-repeat: no-repeat;
      background-position: -60px -30px;
  }

```

- 文本

<div>
<h2>CSS 文本属性</h2>
<table class="dataintable">
  <tbody><tr>
    <th>属性</th>
    <th>描述</th>
  </tr>
  <tr>
    <td><a href="pr_text_color.asp">color</a></td>
    <td>设置文本颜色</td>
  </tr>
  <tr>
    <td><a href="pr_text_direction.asp" title="CSS direction 属性">direction</a></td>
    <td>设置文本方向。</td>
  </tr>
  <tr>
    <td><a href="/css/pr_dim_line-height.asp">line-height</a></td>
    <td>设置行高。</td>
  </tr>
  <tr>
    <td><a href="pr_text_letter-spacing.asp" title="CSS letter-spacing 属性">letter-spacing</a></td>
    <td>设置字符间距。</td>
  </tr>
  <tr>
    <td><a href="pr_text_text-align.asp" title="CSS text-align 属性">text-align</a></td>
    <td>对齐元素中的文本。</td>
  </tr>
  <tr>
    <td><a href="pr_text_text-decoration.asp">text-decoration</a></td>
    <td>向文本添加修饰。</td>
  </tr>
  <tr>
    <td><a href="pr_text_text-indent.asp" title="CSS text-indent 属性">text-indent</a></td>
    <td>缩进元素中文本的首行。</td>
  </tr>
  <tr>
    <td>text-shadow</td>
    <td>设置文本阴影。CSS2 包含该属性，但是 CSS2.1 没有保留该属性。</td>
  </tr>
  <tr>
    <td><a href="pr_text_text-transform.asp">text-transform</a></td>
    <td>控制元素中的字母。</td>
  </tr>
  <tr>
    <td>unicode-bidi</td>
    <td>设置文本方向。</td>
  </tr>
  <tr>
    <td><a href="pr_text_white-space.asp" title="CSS white-space 属性">white-space</a></td>
    <td>设置元素中空白的处理方式。</td>
  </tr>
  <tr>
    <td><a href="pr_text_word-spacing.asp" title="CSS word-spacing 属性">word-spacing</a></td>
    <td>设置字间距。</td>
  </tr>
</tbody></table>
</div>

- 链接

```css
  a:link {text-decoration: none;}
  a:visited {text-decoration: none;}
  a:hover {text-decoration: underline;}
  a:active {text-decoration: underline;}
```

- 列表

<div>
<h2>CSS 列表属性(list)</h2>

<table class="dataintable">
  <tbody><tr>
    <th>属性</th>
    <th>描述</th>
  </tr>
  <tr>
    <td><a href="pr_list-style.asp">list-style</a></td>
    <td>简写属性。用于把所有用于列表的属性设置于一个声明中。</td>
  </tr>
  <tr>
    <td><a href="pr_list-style-image.asp">list-style-image</a></td>
    <td>将图象设置为列表项标志。</td>
  </tr>
  <tr>
    <td><a href="pr_list-style-position.asp">list-style-position</a></td>
    <td>设置列表中列表项标志的位置。</td>
  </tr>
  <tr>
    <td><a href="pr_list-style-type.asp">list-style-type</a></td>
    <td>设置列表项标志的类型。</td>
  </tr>
  
</tbody></table>
</div>


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


