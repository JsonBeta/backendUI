# [BackendUI v1.0.3](https://github.com/JsonBeta/backendUI)

backendUI是一套基于 [BOOTSTRAP](https://github.com/JsonBeta/BOOTSTRAP "BOOTSTRAP")源码编译，在不修改[BOOTSTRAP](https://github.com/JsonBeta/BOOTSTRAP "BOOTSTRAP")原有API的基础上，提供WEB后台项目通用的UI组件；<br/>
主要包括:LAYOUT TABLE FORM GRID BUTTONS ICONS CHARTS等.

To get started, checkout [https://github.com/JsonBeta/backendUI](https://github.com/JsonBeta/backendUI)!



## 快速应用

* [Download the latest release](https://github.com/JsonBeta/backendUI/archive/master.zip).
* Clone the repo: `git clone https://github.com/JsonBeta/backendUI.git`



## BackendUI简介
什么是backendUI？
> backendUI是一套基于BOOTSTRAP源码编译，在不修改BOOTSTRAP原有API的基础上，提供WEB后台项目通用的UI组件；
主要包括:LAYOUT TABLE FORM GRID BUTTONS ICONS CHARTS AND SO ON...
综合效果预览:[docs/examples/apidoc.html](https://github.com/JsonBeta/backendUI/blob/master/docs/examples/apidocs.html)

### backendUI的使用场景？
#### web后台项目

如何快速的应用backendUI?

* 首页需要到项目托管的GITHUB地址： https://github.com/JsonBeta/backendUI download一份源码;
* 将项目中的两个CSS文件放于页面HEAD部分

``` 
<link href="assets/css/bootstrap.css" rel="stylesheet">
<link href="assets/css/bootstrap-responsive.css" rel="stylesheet">
```

* bootstrap原生JS插件合并压缩
	
```
	<script src="assets/js/bootstrap.min.js"></script>
```
	
BackendUI提供的JS插件（按需放置全局LAYOUT模板底部）

    <!-- 表单美化插件 -->
    <script src="assets/js/jquery.uniform.js"></script>
    <!-- 非常强大的SELECT插件 http://ivaynberg.github.io/select2/ -->
    <script src="assets/js/select2.js"></script>
    <!-- jquery 日历插件 -->
    <script src="assets/js/jquery.validationEngine.js"></script>
    <script src="assets/js/jquery.validationEngine-zh_CN.js"></script>
    <!-- 用来生成静态或动态波谱图表效果 -->
    <script src="assets/js/jquery.sparkline.js"></script>
    <!-- 多功能表格插件 -->
    <script src="assets/js/jquery.dataTables.js"></script>
    <!-- 相册 支持TOUCH -->
    <script src="assets/js/touchTouch.jquery.js"></script>
    <!-- 泡泡消息 -->
    <script src="assets/js/jquery.gritter.js"></script>
    <!-- highcharts绘图 包含highcharts.js exporting.js -->
    <script src="assets/js/highcharts.js"></script>
    <script src="assets/js/exporting.js"></script>
    
##使用文档(如何快速构建页面结构)

* 详细介绍

> download backendUI的源码到本地后，找到 [`docs/index.html`](https://github.com/JsonBeta/backendUI/blob/master/docs/index.html)此文件后，浏览器打开即可。 

* examples 使用实例

> 找到 `docs/examples/` 目录，[docs/examples/layout.html](https://github.com/JsonBeta/backendUI/blob/master/docs/examples/layout.html) 此目录提供包括button,icon,grid,widgets等使用实例，可作为参考
  ；另外建议将此目录下layout.html内容作为项目的layout模板

### 你需要编辑源码？
#### 本地需要有LESS编译环境

JAVASCRIPT文件合并压缩(ubuntu),在这之前你需要有NODEJS的运行环境，并安装uglifyjs模块;执行以下2个命令：

```
@cat js/bootstrap-transition.js js/bootstrap-alert.js js/bootstrap-button.js js/bootstrap-carousel.js js/bootstrap-collapse.js js/bootstrap-dropdown.js js/bootstrap-modal.js js/bootstrap-tooltip.js js/bootstrap-popover.js js/bootstrap-scrollspy.js js/bootstrap-tab.js js/bootstrap-typeahead.js js/bootstrap-affix.js > docs/assets/js/bootstrap.js
@./node_modules/.bin/uglifyjs -nc docs/assets/js/bootstrap.js > docs/assets/js/bootstrap.min.js
```
