
```html
    <div id="pannel" >
        <div class="left" >
            left
        </div>
        <div class="right" >
            right
        </div>
        <div class="clear" >
            
        </div>
    </div>
```

```css
    #pannel {
        width: 70%;
        border: 1px solid #ccc;
        background-color: #cecece;
        margin: 10px auto;
        position: relative;
        
        .clear {
            clear: both;
        }
        
        .left {
            width: 30%;
            height: 100%;
            background-color: #fff;
            float: left;
        }
        
        .right {
            width: 70%;
            height: 300px;
            background-color: #ddd;
            float: right;
        }
    }
```