[上一页 异步编程](异步编程.md)

[上一页 Vue编程思考与问题](Vue编程思考与问题.md)

# JS实现异步编程

# JS 如何进行异步编程(异步编程.md)？
``` md
#  1. 通过使用**回调函数**实现异步编程（现在已经过时了），因为难以理解且存在深层回调导致的回调地狱的问题
  [参考资料1](https://developer.mozilla.org/zh-CN/docs/Learn/JavaScript/Asynchronous/Introducing#%E5%9B%9E%E8%B0%83)
```
-  [参考资料1](https://developer.mozilla.org/zh-CN/docs/Learn/JavaScript/Asynchronous/Introducing#%E5%9B%9E%E8%B0%83)

``` md
#  2. 通过 **Promise 对象** 实现异步编程（推荐方法）
  [参考资料1](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Promise)

  [参考资料2](https://github.com/nodejh/nodejh.github.io/issues/23)

  [参考资料3](https://blog.mazey.net/understand-promise)

  [Promise 对象是什么](Promise是什么？.md)

  [Promise 对象如何进行异步编程](Promise的使用方法.md)
```
-  [参考资料1](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Promise)

-  [参考资料2](https://github.com/nodejh/nodejh.github.io/issues/23)

-  [参考资料3](https://blog.mazey.net/understand-promise)

-  [Promise 是什么](Promise是什么？.md)

-  [Promise 对象如何进行异步编程](Promise的使用方法.md)

``` md
#  3. 通过 **async 和 await 关键字**实现异步编程（本质上是对 Promise 的拆封，不如直接用 Promise。）
  [async 参考资料1](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Operators/async_function)

  [await 参考资料2](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Operators/await)

  [async 关键字是什么](是一个用来声明一个函数是异步函数的关键字)

  [await_关键字是什么](是一个**立刻执行所修饰的表达式**，然后**在将后面的代码整体当作一个微任务放入微队列中，等待一个已兑现或已拒绝的 Promise 对象的关键字**，（**注意**）await 只能在**异步函数**或**模块顶层**使用。（**注意**）且 await 修饰的表达式必须要返回一个已兑现或已拒绝的 Promise 对象。否则操作会无法按照你的预期进行。)

  [异步函数 参考资料3](https://blog.csdn.net/ixidof/article/details/7108771)

  [异步函数是什么？](当该函数被调用后，会立即返回。即使该函数的任务没有做完。则该函数为异步函数。)

  [同步函数是什么？](当该函数被调用后，不会立即返回。直到该函数的所有任务全部做完，才会返回。则该函数为同步函数。)

  [async_和_await_如何使用？](必须搭配使用，首先，使用 async 声明一个函数为异步函数，然后使用 await 立刻执行所修饰的表达式，在将后面的代码整体当作一个微任务放如微队列中，等待一个异步兑现或异步拒绝的 Promise 对象。)（**注意**）await 只能在**异步函数**或**模块顶层**使用。（**注意**）且 await 修饰的表达式必须要返回一个已兑现或已拒绝的 Promise 对象。
```
-  [async 参考资料1](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Operators/async_function)

-  [await 参考资料2](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Operators/await)

-  [异步函数 参考资料3](https://blog.csdn.net/ixidof/article/details/7108771)