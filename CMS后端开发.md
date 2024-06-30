[上一页 README](README.md)

# CMS 系统的后端开发三问
``` md
## CMS 系统是什么？
> 1. CMS 系统是 Content Manage Systerm 内容管理系统

> 2. 
```

``` md
## 为什么要开发 CMS 系统？
> 1. 因为一个完整的 CMS 系统，可以让开发人员专注于业务，而不是框架设计，节约开发成本和开发时间。

> 2. 
```


``` md
## 怎么开发 CMS 系统？
> 1. 看后端视频教学

> 2. 后端开发视频地址 百度网盘 Java全栈-30周【完结】

> 3. 看对应的文档解释

> 4. 
```

# CMS 后端开发遇到的问题与解决措施
``` md
## MVC 架构下，Java 项目开发的流程（前提：基本环境配置 以及 springboot 后端框架 配置完成）是什么？
## 基于 Java 的 API 开发流程
> 1. 构建 数据库

> 2. 构建 model `数据模型`层
  （负责与 DB 以及 mapper 层进行通信）

  （获得 数据库 提供的数据，通过构建数据模型实现）

> 3. 构建 mapper `映射`层
  （负责与 model 以及 service 层进行通信）

  （获取 model 数据模型层的数据，通过制定接口，然后通过 XML / 注解 实现接口，获取 model 层的数据）

> 4. 构建 service `服务`层
  （负责与 mapper 以及 controller 层进行通信）

  （获取 mapper 层中的数据，通过调用制定好的接口实现）

> 5. 构建 controller `控制`层
  （负责与 service 以及 view 层进行通信）

  （获取 service 层提供的数据，通过已提供的服务实现）

> 6. 构建 View `视图`层
  （负责与 controller 以及 用户层进行通信）

  （获取 controller 提供的数据，通过已提供的 controller 路径实现）

> **注意1**开发流程为从 1 到 5 。（由于前后端分离，6已经独立出去了）

> **注意2**至于层与层之间如何进行通信，需要自己把握。
```

``` md
## MVC 是什么?
> 1. MVC 是一种软件分层设计架构，Model Controller，View 软件分层设计模式。 

> 2. [参考资料 MVC](https://www.freecodecamp.org/chinese/news/what-does-mvc-mean-in-computer-science/)

> 3. 
```
- [参考资料 MVC](https://www.freecodecamp.org/chinese/news/what-does-mvc-mean-in-computer-science/)

``` md
## JWT 是什么？
> 1. JWT Json Web Token 机制

> 2. [参考资料 JWT](https://www.freecodecamp.org/chinese/news/how-to-sign-and-validate-json-web-tokens/)

> 3. 
```
- [参考资料 JWT](https://www.freecodecamp.org/chinese/news/how-to-sign-and-validate-json-web-tokens/)

``` md
## Mybatis 是什么？
> 1. 
```

``` md
## JPA 是什么？
> 1. 
```

``` md
## Mybatis Plus 是什么？
> 1. 
```

``` md
## 插件 是什么？
> 1. 是一种扩展，为你提供额外的功能

> 2. 
```

``` md
## .XML 是什么？
> 1. 是一种可扩展的标记语言，可以作为一种数据类型，支持跨系统的数据传输。

- 您可以使用 XML 在以不同格式存储相同数据的两个系统之间传输数据。例如，您的网站以 MM/DD/YYYY 格式存储日期，但您的会计系统以 DD/MM/YYYY 格式存储日期。您可以使用 XML 将数据从网站传输到会计系统。您的开发人员可以编写代码自动转换以下内容：

- 将网站数据转换为 XML 格式

- 将 XML 数据转换为会计系统数据

- 将会计系统数据转换回 XML 格式

- 将 XML 数据转换回网站数据

> 2. 
```

``` md
## 为什么使用 XML？
> 1. 因为 XML 可以作为一种数据类型，支持跨系统的数据传输

> 2. 
```


``` md
## 怎么在 Mybatis 中，使用 .xml 文件写 SQL 语句？
> 1. 参考实例文件

> 2. 基本思路：先进行 接口 和 数据模型 的映射，然后通过 XML 标签语言实现具体 SQL 语句。
```