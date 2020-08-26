网格系统 -Grid
=============

## 知识点

* Bootstrap 5 网格系统的学习

## 网格系统

+ 12列布局
+ 6个断点(xs, sm, md, lg, xl, xxl)
+ 灵活的列定义
+ 与容器(container)配合，完成布局

## 实战演习

~~~html
<body>
    <!-- Main Body -->
    <div class="container bg-dark">
        <div class="row">
            <div class="col border bg-light p-3">1</div>
        </div>
        <div class="row">
            <div class="col border bg-light p-3">1</div>
            <div class="col border bg-light p-3">2</div>
        </div>
        <div class="row">
            <div class="col border bg-light p-3">1</div>
            <div class="col border bg-light p-3">2</div>
            <div class="col border bg-light p-3">3</div>
        </div>
        <div class="row">
            <div class="col border bg-light p-3">1</div>
            <!-- 设置单列的宽度比例 6/12 -->
            <div class="col-6 border bg-light p-3">2</div>
            <div class="col border bg-light p-3">3</div>
        </div>
        <div class="row">
            <!-- 响应式布局 -->
            <div class="col col-xl-10 col-lg-8 col-md-6 col-sm-4 border bg-light p-3">1</div>
        </div>
        <div class="row">
            <!-- 响应式布局 -->
            <div class="col col-xl-12 col-lg-10 col-md-8 col-sm-6 border bg-light p-3">1</div>
        </div>
        <div class="row">
            <!-- 响应式布局 -->
            <div class="col col-xl-12 col-lg-10 col-md-8 col-sm-12 border bg-light p-3">1</div>
        </div>
        <div class="row">
            <!-- 响应式布局２列组合 -->
            <div class="col col-xl-6 col-lg-6 col-md-12 col-sm-12 border bg-warning p-3">1</div>
            <div class="col col-xl-6 col-lg-6 col-md-12 col-sm-12 border bg-info p-3">2</div>
        </div>
    </div>
    <hr>
    <p style="text-align: center;">窗口宽度: <span id="width"></span></p>
    <script>
        var widthOutput = document.querySelector('#width');
        function resize() {
            widthOutput.textContent = window.innerWidth;
        }
        window.onresize = resize;
        resize();
    </script>
    <!-- JavaScript -->
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/5.0.0-alpha1/js/bootstrap.bundle.min.js"
        crossorigin="anonymous"></script>
</body>
~~~

## 课程文件

https://github.com/komavideo/LearnBootstrap5

## 小马视频频道

http://komavideo.com
