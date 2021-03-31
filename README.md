# underscore v1.12.0 源码阅读 

1. JavaScript 模块打包器 `rollup.js`
2. 浏览器环境 self === window， 
3. func.length 函数形参长度(会忽略剩余参数)， argument 实参
4. +'1' 会被转换为Number类型
5. DataView
6. Object.prototype.toString.call 可以判断 `String`, `Number`, `Date`, `RegExp`, `Error`, `Symbol`, `ArrayBuffer`, *`Function`, *`isDataView`, `Arguments` `` 
7. 立即执行函数表达式（IIFE）
8. root
    ```JavaScript
    var root = (typeof self == 'object' && self.self == self && self) ||                // 浏览器/Web Worker
               (typeof global == 'object' && global.global == global && global) ||      // Node
               this ||                                                                  // Node vm
               {};                                                                      // 微信小程序
    ```
9. 函数对象
10. 
