[上一页 Vue项目练习经验](Vue项目练习经验.md)

``` md
# [参考资料 各个选项的详细使用方法](https://cn.vuejs.org/guide/introduction.html)
```
-  [参考资料 各个选项的详细使用方法](https://cn.vuejs.org/guide/introduction.html)

``` md
# [参考资料 各个选项的推荐使用顺序](https://v2.cn.vuejs.org/v2/style-guide/#%E7%BB%84%E4%BB%B6-%E5%AE%9E%E4%BE%8B%E7%9A%84%E9%80%89%E9%A1%B9%E7%9A%84%E9%A1%BA%E5%BA%8F%E6%8E%A8%E8%8D%90)
```
-  [参考资料 各个选项的推荐使用顺序](https://v2.cn.vuejs.org/v2/style-guide/#%E7%BB%84%E4%BB%B6-%E5%AE%9E%E4%BE%8B%E7%9A%84%E9%80%89%E9%A1%B9%E7%9A%84%E9%A1%BA%E5%BA%8F%E6%8E%A8%E8%8D%90)

# 常用选项划分
``` js
#  1. 响应式选项
    name: "componentName",
    components: {
      component1,
      component2,
    },
    props: {
      fromParentComponentData: {
        type: String,
        default: ()=>{
          return {

          }
        },
        require: true
      }

    },
    data() {
      return{

      }
    },
    computed: {
      computedData1(){
        const result = {

        },

        return result;
      }
    },
    watch: {
      watchedData: {
        handler(newValue, oldValue){
          // 此处写所需的操作

        },
        deep: true,
      }
    },
    created(){

    },
    mounted(){
      
    }
```

``` js
#  2. 非响应式选项
  methods: {

  }
```