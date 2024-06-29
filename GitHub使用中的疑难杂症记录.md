[上一页 README](README.md)

# GitHub 使用中的疑难杂症记录
- 
``` md
# 本地仓库如何推送至远程仓库
## 建议流程如下
> 1. 在 GtiHub 创建远程仓库。

> 2. 通过 git clone 命令将远程仓库下载至本地文件所在的目录下。

> 3. 通过 VSCode 自带的 Git 操作可视化界面，推送至远程仓库即可。
```
- 
``` md
# Git 如何查看自己的用户信息以及修改（因为连接远程时，需要用户名和用户密码）
## git 命令如下
> 1. 获取当前用户信息
  git config user.name   //获取当前登录的用户
  git config user.email  //获取当前登录用户的邮箱

> 2. 修改当前用户信息
  git config --global user.name 'userName'    // 修改登陆账号，userName为你的git账号
  git config --global user.email 'email'      // 修改登陆邮箱，email为你的git邮箱
  git config --global user.password 'password'  // 修改登陆密码，password为你的git密码

> 3. 清理本地缓存
  git clean -df
```
- 
``` md
# 本地仓库推送至 Github 远程仓库时报错
## git push origin main:main
> 1. fatal: unable to access 'https://github.com/MuNan-HL/SE.git/': Failed to connect to github.com port 443 after 21074 ms: Couldn't connect to server

> 2. 解决办法
  关闭 VSCode 重启
```
- 