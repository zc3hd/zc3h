# zc3h -g

## Description

* 该全局工具，下面有我自己平时使用的全部架子及工具；
* 安装：`npm i zc3h -g`;
* GitHub：[zc3h](https://github.com/zc3hd/zc3h)
* 测试：命令行输入`zc3h` 界面输出：

```json
$ zc3h
*** zc3h 使用说明 ***

命令行输入 : zc3h cli-gulp-epr <pathname>
        cli-gulp-epr 源码地址:https://github.com/zc3hd/cli-gulp-epr

命令行输入 : zc3h cli-wpkEpr-mpa <pathname>
        cli-wpkEpr-mpa 源码地址:https://github.com/zc3hd/cli-wpkEpr-mpa

命令行输入 : zc3h cli-wpkEpr-spa <pathname>
        cli-wpkEpr-spa 源码地址:https://github.com/zc3hd/cli-wpkEpr-spa
```

* `<pathname>`：路径地址，下载架子的路径地址；比如 `./`为当前目录；不输入就为当前路径；



## Config

* 把所有已经在 `github`上有地址的名称，形成架子或工具的`name`配置到 `bin/index`

```js
// 配置：已经在 github上有地址的名称
var arr = [
  "cli-gulp-epr",
  "cli-wpkEpr-mpa",
  "..."
];
```



## Done

* `cli-gulp-epr`：【`gulp+express`】mpa多页面应用cli；[more info](https://github.com/zc3hd/cli-gulp-epr)
* `cli-gulp-koa`：【`gulp+koa`】mpa多页面应用cli；[more info](https://github.com/zc3hd/cli-gulp-koa)
* `cli-wpkEpr-mpa`：【`webpack+express`】mpa多页面应用cli；[more info](https://github.com/zc3hd/cli-wpkEpr-mpa)
* `cli-wpkEpr-spa`：【`webpack+express`】vue spa多页面应用cli；[more info](https://github.com/zc3hd/cli-wpkEpr-spa)



## Tips

* 开发时如何选择用哪个cli？

* 确定项目是 【单页面SPA】 或【多页面MPA】？

* 单页面SPA：vue技术栈首选，这个时候使用router和vuex才有意义；

  * 【推荐使用 cli-wpkEpr-spa 】处理 **.vue 单文件组件
  * 如果不处理**.vue 单文件组件，使用 cli-wpkEpr-mpa （CSS和JS打包在一起）和 【推荐使用】cli-gulp-epr  都可以；（参考说明：https://github.com/zc3hd/demo_vue/tree/master/src_webapp/demo_008）

* 多页面MPA：使用 cli-wpkEpr-mpa （CSS和JS打包在一起）和 【推荐使用】cli-gulp-epr  都可以；

  * 如果使用vue，那么router和vuex将没有意义，代替的就是真实的页面转跳（不是路由）和本地存储；一个页面就是一个vm实例，使用指令等；vue.js从页面中引入；和使用JQ一样；

    