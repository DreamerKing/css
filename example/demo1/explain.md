# 关键代码  
```css
        .box {
            border: 20px solid hsla(0, 0%, 100%, .4);
            border-radius: 20px;
            background-clip: padding-box;
        }         
```

background-clip的取值有`border-box`、`padding-box`和`content-box`,为了防止背景浸入边框,所以要把它的值设为`padding-box`。