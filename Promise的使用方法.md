[上一页 JS实现异步编程](JS实现异步编程.md)

# Promise 的使用方法
``` md
#  1. 掌握 then 的正确使用，使用 .then(()={})，必须确保 then 能得到一个已兑现的 Promise 对象。
```

``` md
#  2. 掌握 catch 的正确使用，使用 .catch(()={})，必须确保 catch 能得到一个已拒绝的 Promise 对象。
```

``` md
#  3. Promise 对象的获取方法：
```

``` js
  // 如何实例化一个已兑现的 Promise 对象
  new Promise((resolvePromise, rejectPromise)=>{
    // ...

    resolve();
  });

  // 如何实例化一个已拒绝的 Promise 对象
  new Promise((resolvePromise, rejectPromise)=>{
    // ...

    reject();
  })

  // Promise 搭配 then 和 catch 实现异步编程的示例
  this.dataLinkInterface()
  // 使用 .then(()={})，必须确保 then 能得到一个已兑现的 Promise 对象。
  .then((resolveDataLinkInterface)=>{
    // ...
    console.log(resolveDataLinkInterface, "resolveDataLinkInterface");
  })
  // 使用 .catch(()={})，必须确保 catch 能得到一个已拒绝的 Promise 对象。
  .catch((rejectDataLinkInterface)=>{

  })

  dataLinkInterface(){
    return new Promise((resolvePromise, rejectPromise)=>{
      const dataLinkInterfaceParams = {
        // ...
      };

      // 此处模仿实际项目中前端通过 axios 进行的数据联调
      interface(dataLinkInterfaceParams)
      .then((resolveInterface)=>{
        // ...
        console.log(resolveInterface, "resolveInterface");

        // 为后续的 then 方法提供一个已兑现的 Promise 对象
        resolvePromise();
      })
      .catch((rejectInterface)=>{
        // ...
        console.log(rejectInterface, "rejectInterface");
        
        // 为后续的 catch 方法提供一个已拒绝的 Promise 对象
        rejectPromise();
      })
    });

  // Promise 搭配 then 和 catch 实现异步编程的理论依据
  // 通过 axios 进行 HTTP 通信时，axios 依赖给你返回的数据本身就是一个 已兑现或者已拒绝的 Promise 对象，因此你可以不需要自己实例化并返回一个 Promise 对象。
  // 但是你在进行异步编程时，你必须提供一个 Promise 对象，才可以利用 then 或 catch 实现异步编程。
  }
```
