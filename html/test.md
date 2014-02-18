

```html
<div id="header">
    <h1>百度推广</h1>
</div>
<div id="nav">
    
</div>
<div id="main-wrapper">
    <div class="left" >
        <h2>账户树</h2>
        <ul>
            <li>计划1</li>
            <li>计划2</li>
            <li>计划3</li>
        </ul>
    </div>
    <div class="right" id="main">管理信息</div>
</div>

<div id="footer">Copyright @baidu.com</div>
```


样式

```css

#header {
    background-color: skyblue;
    height: 70px;
    color: #FFF;
}

#main-wrapper {
    .left {
        width: 200px;
        float: left;
    }
    
    .right {
        margin-left: 200px;
        background-color: #dedede;
        min-height: 200px;
    }
}


#footer {
    background-color: lightblue;
    width: 100%;
    position: abosolute;
    bottom: 0px;
}

```