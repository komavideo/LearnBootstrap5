页面的断点 - Breakpoints
=======================

## 知识点

* 了解Bootstrap5中的断点设计

## 官网

https://v5.getbootstrap.com/docs/5.0/layout/breakpoints/

## 断点的设计理由

+ 实现响应式页面
+ 根据媒体查询变换CSS
+ 能够实现移动优先

## Bootstrap中的断点

+ 超小：0-576px
+ 小：sm-, ≥576px
+ 中：md-, ≥768px
+ 大：lg-, ≥992px
+ 超大：xl-, ≥1200px
+ 超超大：xxl-, ≥1400px

## 源代码： _variables.scss

https://github.com/twbs/bootstrap

~~~scss
// scss-docs-start grid-breakpoints
$grid-breakpoints: (
  xs: 0,
  sm: 576px,
  md: 768px,
  lg: 992px,
  xl: 1200px,
  xxl: 1400px
) !default;
// scss-docs-end grid-breakpoints
~~~

## 课程文件

https://github.com/komavideo/LearnBootstrap5

## 小马视频频道

http://komavideo.com
