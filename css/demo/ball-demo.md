
<div id="wrapper">
    <div id="pannel" >
        <div class="ball" id="ball-1" >
            
        </div>
        <div class="ball" id="ball-2">
            
        </div>
        <div class="ball" id="ball-3">
            
        </div>
        <div class="ball" id="ball-4" >
            
        </div>
    </div>

</div>

<style>

#pannel {
    width: 70%;
    height: 500px;
    border: 1px solid #ccc;
    background-color: #cecece;
    margin: 10px auto;
    position: relative;
    
    .ball {
        width: 50px;
        height: 50px;
        background-color: #ff0000;
        position: absolute;
        border-radius: 25px;
        left: 0;
        top: 0;
    }
    
    #ball {
        
        &-2 {
            left: 200px;
        }
        
        &-3 {
            top: 200px;
        }
        
        &-4 {
            left: 200px;
            top: 200px;
        }
    }
}

</style>

```html
    <div id="pannel" >
        <div class="ball" id="ball-1" >
            
        </div>
        <div class="ball" id="ball-2">
            
        </div>
        <div class="ball" id="ball-3">
            
        </div>
        <div class="ball" id="ball-4" >
            
        </div>
    </div>
```

``` css
#pannel {
    width: 70%;
    height: 500px;
    border: 1px solid #ccc;
    background-color: #cecece;
    margin: 10px auto;
    position: relative;
    
    .ball {
        width: 50px;
        height: 50px;
        background-color: #ff0000;
        position: absolute;
        border-radius: 25px;
        left: 0;
        top: 0;
    }
    
    #ball {
        
        &-2 {
            left: 200px;
        }
        
        &-3 {
            top: 200px;
        }
        
        &-4 {
            left: 200px;
            top: 200px;
        }
    }
}
```
