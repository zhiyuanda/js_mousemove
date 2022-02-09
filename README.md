>  参考来源：
>
> [JavaScript基础语法-dom-bom-js-es6新语法-jQuery-数据可视化echarts黑马pink老师前端入门基础视频教程(500多集)持续_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1Sy4y1C7ha?p=244&spm_id_from=pageDriver)

## 网页GitHub地址如下：（若加载较慢建议刷新后耐心等待一会~）

[js_mousemove](https://jiang-lijun.github.io/js_mousemove/)

## 主要功能：

鼠标移动时，动图小人会随着鼠标一起移动

## 网页代码如下：

### HTMLHTML+CSS+JS：

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>js_mousemove</title>
    <style>
        img {
            position: absolute;
            width: 70px;
            top: 2px;
        }
    </style>
</head>
<body>
    <img src="pic.gif" alt="">
    <script>
        var img = document.querySelector('img');
        document.addEventListener('mousemove',function(e) {
            var x = e.pageX;
            var y = e.pageY;
            img.style.left = x - 35 + 'px';
            img.style.top = y - 40 + 'px';
        })
    </script>
</body>
</html>
```

