## 关于VueComponent： 
##

### 1.school组件本质时一个名为VueComponent的构造函数，且不是程序员定义的,是Vue.extend生成的 ###

### 2.我们只需要写<school></school>，Vue解析时会帮我们创建school组件的实例对象，即Vue帮我们执行的：new VueComponent(options) ###

### 3.特别注意：每次调用Vue.extend，返回的都是一个全新的VueComponent！！！ ###

### 4.关于this指向：
    （1）组件配置中：
        data函数、methods中的函数、watch中的函数、computed中的函数 它们的this都是[VueComponent实例对象]
    （2）new Vue()配置中：
        data函数、methods中的函数、watch中的函数、computed中的函数 它们的this都是[Vue实例对象]
 ###

 ### 5.VueComponent的实例对象，以后简称vc(也可称之为：组件实例对象)。Vue的实例对象，以后简称vm ###