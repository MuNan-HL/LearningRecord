[上一页 Vue项目练习经验](Vue项目练习经验.md)

[上一页 前端开发工具](前端开发工具.md)

# Axios 一个基于 promise 对象的，可以用于浏览器和node.js的网络请求库

``` md
  [参考资料 官网](https://axios-http.com/zh/docs/intro)

  [参考资料 GitHub](https://github.com/axios/axios)
```
- [参考资料 官网](https://axios-http.com/zh/docs/intro)

- [参考资料 GitHub](https://github.com/axios/axios)

``` md
# axios 是什么？
> Axios 是一个基于 promise 对象的，可以用于浏览器和node.js的网络请求库，作用于node.js 和浏览器中。 它是 isomorphic 的(即同一套代码可以运行在浏览器和node.js中)。在服务端它使用原生 node.js http 模块, 而在客户端 (浏览端) 则使用 XMLHttpRequests。
```

``` md
# 为什么要使用 axios 网络请求库？
> 因为 axios 时一个基于 promise 对象的，可以用于浏览器和node.js的网络请求库
```

``` js
# 怎么使用 axios 网络请求库？
import request from "#/router/axios"

// get 请求
export function interface(params) {
  return request({
    method: "get",
    url: "",
    params: params
  })
}

// post 请求
export function interface(data) {
  return request({
    method: "post",
    url: "",
    data: data
  })
}
```