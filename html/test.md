

```html
<div id="header" >
    <h1 class="logo" >
         百度推广
    </h1>
    <ul class="horiz-nav">
        <li>首页</li>
        <li>便捷管理</li>
        <li>推广管理</li>
    </ul>
</div>

<div id="wrapper">
    <div class="left">
        <h1>
            账户树
        </h1>
        <ul>
            <li>1</li>
            <li>2</li>
            <li>3</li>
        </ul>
    </div>
    <div class="right">
        right
    </div> 
    <div class="clear" >
        
    </div>
</div>

<div id="footer" >
    <div class="copyright" >
        copyright @ baidu.com
    </div>
</div> 
```


样式

```css

#header {
    height: 90px;
    background-color: #264597;
    position: relative;
    
    .logo {
        margin: 0;
        color: #fff;
        position: absolute;
        bottom: 10px;
        left: 5px;
        font-size: 20px;
    }
    
    .horiz-nav {
        list-style: none;
        margin: 0;
        position: absolute;
        left: 100px;
        bottom: 0;
        li {
            display: inline-block;
            border: 1px solid;
            border-bottom: 0;
            padding: 5px;
            margin: 0;
            background-color: #5279de;
            color: #FFF;
        }
    }
}

#wrapper {
    border: 1px solid #ccc;
    .left {
        float: left;
        width: 200px;
        border-right: 1px solid #ccc;
    }
    .right {
        margin-left: 200px;
        height: 90px;
        padding: 10px;
    }
    .clear {
        clear: both;
    }
}

#footer {
    background-color: #dedede;
    .copyright {
        width: 200px;
        line-height: 50px;
        margin: 0px auto;
    }
}


```