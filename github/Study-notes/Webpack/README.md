# demos


webpack 知识点：

命令：

npm init -y  // 初始化文件（默认值）yes


node -v   // 版本号

npm -v  

npm install -g less   // less 包

less demo.less > demo.css   // less 转换成 css

npm install -g uglify-js  // js 包

uglifyjs demo.js -o demo.min.js  // 压缩js


npm install -g cnpm --registry=https://registry.npm.taobao.org   // 淘宝镜像

cnpm install webpack -g  // 安装webpack
 
cnpm install webpack-cli -g   // 安装webpack-cli

webpack  // 打包

webpack demo.js -o bundle.js  打包demo.js  输出bundle.js

npm init   // 初始化文件（默认值）  npm init -y  //跳过询问

cnpm install webpack --save-dev  // 开发环境下载webpack

cnpm install jquery -D  //下载jQuery

webpack demo.js -o bundle.js --mode development   //开发环境（警告消失）

npm install style-loader less-loader css-loader less --save-dev  // 下载loader less


（"scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "dev": "webpack --mode development",
    "prod": "webpack --mode production"
  },）
npm run dev   // 执行 
 
npm run prod  // 执行 


拿到项目执行  npm install  会按照 package.json 里边的版本号下载初始化

$ npm install lodash-es -D  //lodash 库


js-tree-shaking 深度压缩 tree-shaking网址：https://www.npmjs.com/package/webpack-deep-scope-plugin

npm install webpack-deep-scope-plugin -D    // webpack-deep-scope-plugin 插件 深度tree-shaking


css-tree-shaking 样式深度压缩 mini-css-extract-plugin  网址 https://www.npmjs.com/package/mini-css-extract-plugin

npm install --save-dev mini-css-extract-plugin //下载插件


npm install -g browserify   // 下载包（浏览器不支持exports）
 
browserify index.js -o bundle.js  // 输出js

npm install uniq  // 下载包（去重排序）
