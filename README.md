# neko0-web-advance-module

## install

`npm i neko0-web-advance-module -S`

`cnpm i neko0-web-advance-module -S`

npm package page: https://www.npmjs.com/package/neko0-web-advance-module

在 Vue 中使用 App.vue 中加入以下内容

``` html
<style lang="scss">
@import 'neko0-web-advance-module/scss/reset.scss';
@import 'neko0-web-advance-module/scss/main.scss';
@import 'neko0-web-advance-module/scss/color.scss';
</style>
```

也可以根据此方法 选择性添加 自己需要的文件

## color.scss

基于 [Muse UI](https://muse-ui.org/#/zh-CN/color) 修改 

    Muse UI的是Less用的，这里将其改为了SCSS
    可以直接于官方网址内的Color参考颜色并且复制颜
    色名


## helpers.scss

主要灵感源于 [Emmet](https://emmet.io/)

    
    类似于在 HTML Tag 的 class 中直接编写 Emmet 的 CSS 部分
    position 之类定义后还要定义 top 等其他样式数值的个人认为还是单独写在一起的可读性比较好
    所以暂时只收录了常用的部分
    加入了一些 Neko0 自用样式
    之后有需求可能会继续添加(包括position)

## package.scss

    修改了一些第三方包本身有所缺陷的地方

## spacing.scss

基于 [Vuetify](https://vuetifyjs.com/zh-Hans/layout/spacing) 修改 

    Vuetify的是Stylus用的，这里将其改为了SCSS适用的并拓展
    将margin或者padding应用于一个元素，范围在 0到5 之间。
    每个尺寸增量都设计成与常用Material Design间距对齐。
    这些类可以使用m-{property}{direction}-{size}这个格式来应用。

    占位符 property 用来设置间距的类型：
    m - 对应 margin
    p - 对应 padding

    占位符 direction 指定属性所应用到的方向：
    t - 对应margin-top或者padding-top属性
    b - 对应margin-bottom or padding-bottom
    l - 对应margin-left or padding-left
    r - 对应margin-right or padding-right
    x - 同时对应*-left和*-right属性
    y - 同时对应*-top和*-bottom属性

    占位符 size 控制属性的增量：
    0 - 将margin或者padding设置为0，会使这些属性被删除
    1 - 将margin或者padding属性设置为$spacer * .25
    2 - 将margin或者padding属性设置为$spacer * .5
    3 - 将margin或者padding属性设置为$spacer
    4 - 将margin或者padding属性设置为$spacer * 1.5
    5 - 将margin或者padding属性设置为$spacer * 3

## reset.scss 

    个人规范意义的 初始化用的 scss 文件

## main.scss

包含了

    package.scss
    helpers.scss
    spacing.scss