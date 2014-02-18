## less基础

### 变量定义

```css
    @nice-blue: #5B83AD;
    @light-blue: @nice-blue + #111;
    #header { color: @light-blue; }
```

输出结果为

```css
    #header { color: #6c94be; }
```

### mixin

```css
    .bordered {
      border-top: dotted 1px black;
      border-bottom: solid 2px black;
    }

    #menu a {
      color: #111;
      .bordered;
    }
```

输出结果为

```css
    #menu a {
      color: #111;
      border-top: dotted 1px black;
      border-bottom: solid 2px black;
    }
```

### 带参混合

```css
    .border-radius (@radius) {
      border-radius: @radius;
      -moz-border-radius: @radius;
      -webkit-border-radius: @radius;
    }
    #header {
      .border-radius(4px);
    }
```

### 嵌套规则
> less 可以基于dom元素的层次结构实现css的嵌套定义

```css
    #header {
      color: black;

      .navigation {
        font-size: 12px;
      }

      .logo {
        width: 300px;
        &:hover { text-decoration: none }
      }
    }
```

输出结果为

```css
    #header {
      color: black;
    }
    #header .navigation {
      font-size: 12px;
    }
    #header .logo {
      width: 300px;
    }
    #header .logo:hover {
      text-decoration: none;
    }
```

> 以下内容自行参考文档学习

- 条件混合
- 变量作用域
- 变量操作符
- 内嵌函数
- 忽略编译
- js语句执行

> 掌握less的核心语法；目标是为了写出可读性更高，执行效率更高，管理更方便的前端样式代码；

[less 在线练习](http://fiddlesalad.com/less/)