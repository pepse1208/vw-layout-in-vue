# vw-layout-in-vue

在vue项目中使用vw实现移动端适配。截止目前最前卫的适配方式，手淘团队使用并推荐

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report

# run unit tests
npm run unit

# run all tests
npm test
```
#总结

盒子（容器）都要添加容器宽度比，有一个默认的结构。图片宽度用px高写成auto，因为有了宽度比所以不会变形
使用宽度比的时候    aspectratio   aspectratio-content 是必写的

<div aspectratio>
    <div aspectratio-content>
    </div>
</div>

不想把px转换为vw，可以添加指定的类名

1px解决方案，针对于border   border-image  background-image

引入vw兼容js  ➕script

[aspectratio]表示自定义属性 它和类名所起的作用是相同的，
定义class时 style里写 .classname。如果标签内写的是自定义属性那么style里就写 [aspectratio]。大漠就喜欢这样用
