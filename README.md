# MINA-Gulp-Template
微信小程序gulp构建模板

### start

```shell
nmp install
```
```shell
gulp build:dev
```
生成测试环境代码到目录下的wechat文件夹
用微信小程序开发者工具打开wechat文件夹，这就是工程的测试环境代码。


### watch
在开发中是用watch命令实时监听文件变化，而小程序开发者工具会自动刷新。

```shell
gulp watch
```

### build
‘打包’命令，生成各自环境的代码

```shell
gulp build:dev
```

```shell
gulp build:pre
```

而在工程中，可以利用DEBUG变量来读取不同的代码，比如配置不同的数据库地址、url...
```js
const isDebug = `DEBUG` === `dev`
if (isDebug) {} else {}
...
```

