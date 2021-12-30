# 课程概述

- 哪些部分？—— API，数据存储，登录，日志，安全

- 技术？—— http stream session mysql redis nginx pm2



# nvm 使用

- `nvm list` 查看所有 node 版本

- `nvm install v10.13.0` 安装指定版本

- `nvm use --delete-prefix 10.13.0` 切换到指定版本



# nodejs 和 js 区别

es 定义了语法，nodejs 和 js 都必须遵守，包括变量定义，循环，判断，函数，原型和原型链，作用域和闭包，异步。*语法规范，没有实际价值*。

不能监听 click 事件，不能发送 ajax 请求，不能操作 DOM

js = es + **Web API**（DOM，BOM，事件绑定，Ajax）

nodejs = es + **Nodejs API**（处理 http，处理文件）



# commonjs

```js
// 📁 a.js
function add(x, y) { return x + y }
function mul(x, y) { return x * y }
module.exports = { add, mul }

// 📁 b.js
const { add, mul } = require('./a')
console.log( add(3, 4) )    // 7
console.log( mul(3, 4) )    // 12
```



# Debug（TODO）

- `Run and Debug` —— 以 package.json 的 main 属性对应路径开始 debug



# server 开发和前端开发区别

- 服务稳定性

- 安全
  
  - xss 攻击、sql 注入

- 考虑内存和 CPU（稀缺资源）
  
  - 使用 stream 写日志，使用 redis 存 session

- 日志记录
  
  - 记录、存储、分析

- 集群和服务拆分
  
  - 通过扩展机器和服务拆分来承载大流量



# 流程

定目标，定需求，定 UI 设计，定技术方案，开发，联调，测试，上线，结果评估
