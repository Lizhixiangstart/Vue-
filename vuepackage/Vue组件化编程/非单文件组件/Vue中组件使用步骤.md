## Vue中使用组件的三大步骤： 
    一、定义组件(创建组件)
    二、注册组件
    三、使用组件(写组件标签)
##

### 一、如何定义一个组件？ 
    使用Vue.extend(ptions)创建，其中options和new Vue({options})时传入的那个options几乎一样，但区别如下：
        1.el不要写，为什么？——最终所有的组件都要经过一个vm的管理，由vm中的el决定服务哪个容器
        2.data必须写成函数，为什么？——避免组件被复用时，数据存在引用关系
        备注：使用template可以配置组件结构
###

### 二、如何注册组件？ 
    1.局部注册：靠new Vue的时候传入components配置项
    2.全局注册：靠Vue.component('组件名',组件)
###

### 三、编写组件标签 
    <school></school>
    <student></student>
###