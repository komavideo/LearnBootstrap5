Media queries - 必须了解的媒体查询
===============================

## 知识点

* 使用CSS的媒体查询功能定制浏览器

## 官网

https://developer.mozilla.org/zh-CN/docs/Web/Guide/CSS/Media_queries

## 实战演习

```html
<!-- 所有设备通用样式单 -->
<link rel="stylesheet" src="styles1.css" media="all" />
<!-- 屏幕专用样式单 -->
<link rel="stylesheet" src="styles2.css" media="screen" />
<!-- 打印专用样式单 -->
<link rel="stylesheet" src="styles3.css" media="print" />
```

## index.html

```html
<!DOCTYPE html>
<html lang="zh">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        /* 超小屏幕 */
        @media (max-width: 576px) {
            .myCSS {
                font-size: 16px;
                color: orange;
            }
        }
        /* 智能手机 */
        @media (min-width: 576px) {
            .myCSS {
                font-size: 24px;
                color: blue;
            }
        }
        /* 中屏平板 */
        @media (min-width: 768px) {
            .myCSS {
                font-size: 32px;
                color: green;
            }
        }
        /* 小型显示器 */
        @media (min-width: 992px) {
            .myCSS {
                font-size: 48px;
                color: red;
            }
        }
        /* 大型显示器 */
        @media (min-width: 1598px) {
            .myCSS {
                font-size: 64px;
                color: black;
            }
        }
    </style>
</head>
<body>
    <span class="myCSS">我爱Bootstrap 5.</span>
    <p>窗口宽度: <span id="width"></span></p>
    <script>
        var widthOutput = document.querySelector('#width');
        function resize() {
            widthOutput.textContent = window.innerWidth;
        }
        window.onresize = resize;
        resize();
    </script>
</body>
</html>
```

## 课程文件

https://github.com/komavideo/LearnBootstrap5

## 小马视频频道

http://komavideo.com
