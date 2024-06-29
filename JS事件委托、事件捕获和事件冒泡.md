[上一页 Vue思考](Vue思考.md)

[上一页 Vue 项目练习经验](Vue项目练习经验.md)

# JS事件委托、事件捕获和事件冒泡

# 是什么？
``` md
#  1. 事件是什么？
    例如 
    -  用户选择、点击或将光标悬停在某一元素上。
    -  用户在键盘中按下某个按键。
    -  用户调整浏览器窗口的大小或者关闭浏览器窗口。
    -  网页结束加载。
    -  表单提交。
    -  视频播放、暂停或结束。
    -  发生错误

    [参考资料1](https://developer.mozilla.org/zh-CN/docs/Learn/JavaScript/Building_blocks/Events#%E4%BB%80%E4%B9%88%E6%98%AF%E4%BA%8B%E4%BB%B6%EF%BC%9F)
```
-  [参考资料1](https://developer.mozilla.org/zh-CN/docs/Learn/JavaScript/Building_blocks/Events#%E4%BB%80%E4%B9%88%E6%98%AF%E4%BA%8B%E4%BB%B6%EF%BC%9F)

``` md
#  2. 事件冒泡是什么？
    事件冒泡是一种**事件传播的处理机制 事件触发顺序是由内向外依次触发。**，**注意 有时你需要[阻止事件冒泡](阻止事件冒泡.md)**

    [参考资料1](https://developer.mozilla.org/zh-CN/docs/Learn/JavaScript/Building_blocks/Events#%E4%BA%8B%E4%BB%B6%E5%AF%B9%E8%B1%A1)
```
-  [阻止事件冒泡](阻止事件冒泡.md)

-  [参考资料1](https://developer.mozilla.org/zh-CN/docs/Learn/JavaScript/Building_blocks/Events#%E4%BA%8B%E4%BB%B6%E5%86%92%E6%B3%A1)

``` md
#  3. 事件捕获是什么？
    事件捕获也是一种事件传播的处理机制，**事件捕获的事件触发顺序是是由外向内依次触发**。**注意 事件捕获默认是禁用的**，事件捕获和事件冒泡属于历史遗留，分别代表了网景和IE浏览器的事件传播处理机制。

    [参考资料1](https://developer.mozilla.org/zh-CN/docs/Learn/JavaScript/Building_blocks/Events#%E4%BA%8B%E4%BB%B6%E5%86%92%E6%B3%A1)
```
-  [参考资料1](https://developer.mozilla.org/zh-CN/docs/Learn/JavaScript/Building_blocks/Events#%E4%BA%8B%E4%BB%B6%E5%86%92%E6%B3%A1)

``` md
#  4. 事件委托是什么？
    **事件委托是事件冒泡机制的一种使用方法**，当我们想在用户与大量的子元素中的任何一个互动时运行一些代码时，我们在它们的父元素上设置事件监听器，让发生在它们身上的事件冒泡到它们的父元素上，而不必在每个子元素上单独设置事件监听器。
```