# zc3h -g

## Description

* 该全局工具，下面有我自己平时使用的全部架子及工具；
* 安装：`npm i zc3h -g`;
* 测试：命令行输入`zc3h` 界面输出：

```json
$ zc3h
*** Welcome AV8day ***

Usage : zc3h cli-gulp-epr <pathname>
        cli-gulp 源码地址:https://github.com/zc3hd/cli-gulp-epr

Usage : zc3h test_1 <pathname>
        test_1 源码地址:https://github.com/zc3hd/test_1

Usage : zc3h test_2 <pathname>
        test_2 源码地址:https://github.com/zc3hd/test_2
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
* `cli-wpkEpr-mpa`：【`webpack+express`】mpa多页面应用cli；[more info](https://github.com/zc3hd/cli-wpkEpr-mpa)

* `cli-wpkEpr-spa`：【`webpack+express`】vue spa多页面应用cli；[more info](https://github.com/zc3hd/cli-wpkEpr-spa)



## Tips

