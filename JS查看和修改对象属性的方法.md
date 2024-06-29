[上一页 Vue思考](Vue思考.md)

# JS 增删改查对象属性的方法
``` js
1. JS 怎么声明一个对象
  // 第一种 大括号 {} 字面量
  let obj = {
    'name' : 'meng',
    'age' : 18
  }

  // 第二种 new 关键字实例化一个对象
  let obj = new Object({ 
  'name' : 'meng', 
  'age' : '18' 
  })

  // 第三种 以一个现有对象作为原型，创建一个新对象。
  var common = { '国籍':'中国',hairColor:'black'}
  var person = Object.create(common)
```

``` js
2.  JS 怎么新增对象的属性
  // 第一种 直接新增
  obj.name = 'meng' // 修改属性

  // 第二种 批量新增
  Object.assign( obj, {'name':'meng', 'age': '18'})
```

``` js
3.  JS 怎么删除对象中的属性
  let obj = {
    name: 'meng',
    age: '18',
    gender: 'man'
  }
  obj.name = undefined // 把 name 属性设置为 undefined
  delete obj.name // 删除属性
```

``` js
4.  JS 怎么修改对象的属性
  // 第一种 直接修改
  obj.name = 'meng' // 修改属性

  // 第二种 批量修改
  Object.assign( obj, {'name':'meng', 'age': '18'})
```

``` js
5.  JS 怎么访问对象中的属性
  // 第一种 方括号
  obj['key']

  // 第二种 点运算
  obj.key
```

``` js
6. JS 怎么查看对象中的属性
  let obj = {
    name: 'meng',
    age: 18
  };
  // 查看所有键
  Object.keys(obj) 

  // 查看所有值
  Object.values(obj) 
  
  // 查看键和值
  Object.entries(obj) 
```
-  [参考资料 juejin](https://juejin.cn/post/7036759316510015519)

-  [参考资料 MDN](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Object)