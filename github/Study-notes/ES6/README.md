# demos


JS模块化 AMD  CMD  ESM

AMD : 前置加载  先加载

CMD : 后加载

ESM :



模块引用写法：es6

m1.js:

import sum from './sum';
console.log(sum(2,4));

m2.js:

export default function sum(a,b){
    return a+b;
}

// 导出模块

var sum = 1;
export {
   sum
}


// 引用文件 模块 库

import XX from ''



ES6 转 ES5

$ npm install @babel/core   // babel 下载

$ npm install @babel/preset-env    // babel集合 下载

$ npm install @babel/cli  // cli 脚手架
 
$ npx babel 1-letconst.js -o 1-newletconst.js  // ES6 转 ES5  输出文件

$ npx babel 1-letconst.js -o 1-newletconst.js --watch  // ES6 转 ES5  输出文件 实时监控

let : 变量

const: 常量

...arg: 数组


数据转成字符串： JSON.stringify(data);

字符串转成数组： JSON.PARSE(res);


let sum = (a, b) => ({a: a, b: b});

sum(10, 20);


let sum = x => y => z => x + y + z;

sum(1)(2)(3);


let sum = () => {console.log(this)}; // 不能写anguments

输出 ： window
