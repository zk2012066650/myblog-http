
# 开发配置

## http

koa2-generator 安装启动项目

``` js
npm install -g koa-generator
koa2 -e http  //e启用ejs模板
cd http
npm install
npm start //或
node bin/www
```

cross-env 安装（作用：设置环境变量）
debug 根据不同的运行打印不同的日志

``` js
npm install cross-env -D

package.json -- // 配置文件名
"dev": "set DEBUG=dev & cross-env NODE_ENV=development nodemon bin/www"
```

---

## www

react-create-app 安装及启动项目

``` js
npm install -g create-react-app
create-react-app --version
create-react-app www
cd www
npm install
npm start
```

scss 安装及配置

``` js
npm install style-loader css-loader sass-loader node-sass -D

cd www/node-modules/react-scripts/config/webpack.config.js //配置地址
// ** STOP ** Are you adding a new loader?
// Make sure to add the new loader(s) before the "file" loader.
{
test: /\.scss$/,
use: ['style-loader', 'css-loader', 'sass-loader']
},

```

react-router-dom 安装

``` js
npm install react-router-dom -S
```

axios 安装

``` js
npm install axios -S
```

antd 安装

``` js
npm install antd -D
```

绝对路径配置

``` js
cd www/node-modules/react-scripts/config/webpack.config.js //配置地址

alias: {
    '@':path.resolve('src'),
    ...
}
```
