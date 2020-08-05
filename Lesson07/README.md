容器的概念 - Containers
======================

## Bootstrap更新进度

https://github.com/twbs/bootstrap/releases  

## 知识点

* 了解Bootstrap5中容器的设计

## 容器设计的目的

控制页面内容显示的宽度

## 容器的类型

+ .container: 自动响应页面宽度
+ .container-fluid: 最大适应页面宽度，即:100%
+ .container-{breakpoint}: 根据断点适应页面宽度(sm, md, lg, xl, xxl)

## 实战演习

~~~html
<div class="container border border-success p-2 mb-2">.container</div>
<div class="container-sm border border-success p-2 mb-2">.container-sm(≥576px)</div>
<div class="container-md border border-success p-2 mb-2">.container-md(≥768px)</div>
<div class="container-lg border border-success p-2 mb-2">.container-lg(≥992px)</div>
<div class="container-xl border border-success p-2 mb-2">.container-xl(≥1200px)</div>
<div class="container-xxl border border-success p-2 mb-2">.container-xxl(≥1400px)</div>
<div class="container-fluid border border-success p-2 mb-2">.container-fluid</div>
<hr>
<p>窗口宽度: <span id="width"></span></p>
<script>
    var widthOutput = document.querySelector('#width');
    function resize() {
        widthOutput.textContent = window.innerWidth;
    }
    window.onresize = resize;
    resize();
</script>
~~~

## 课程文件

https://github.com/komavideo/LearnBootstrap5

## 小马视频频道

http://komavideo.com
