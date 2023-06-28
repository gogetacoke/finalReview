# 单选题

1. Vue实例对象中能够监听状态变化的参数是（ ）。 

   A. watch

   B. filters

   C. watching

   D. components

   > A 

2. 在watch监听中设置（），可以实现深度监听的功能。 

   A. dirty:true 

   B. deep:true

   C. watch:true 

   D. watcher:true

   > B 

3. 下列指令中，不能实现条件判断的是（ ）。 

   A. v-if

   B. v-else

   C. v-show

   D. v-bind

   > D 

4. 在 Vue.js 中，列表渲染使用的是（ ）指令。 

   A. v-on

   B. v-for

   C. v-if

   D. v-model

   > B 

5. 下列不属于 Vue.js 为 v-model 指令提供的修饰符的是（ ）。 

   A. lazy

   B. number

   C. self

   D. trim

   > C 

6. 如果在内联语句中需要获取原生的 DOM 事件对象，可以将特殊变量（ ）传入方法中。

   A. $event

   B. $this

   C. event

   D. this

   > A 

7. 下列对于 v-show 指令的描述错误的是（ ） 

   A. v-show 指令是根据表达式的值来判断是否显示或隐藏 DOM 元素

   B. 使用 v-show 指令的元素都始终会被渲染并保留在 DOM 中

   C. 绑定值的改变只是切换元素的 CSS 属性 display

   D. 如果在运行时条件很少改变，则需要使用 v-show

   > D 

8. 下列不属于 v-on 指令中的事件修饰符的是（ ）。 

   A. .stop

   B. .prevent

   C. .get

   D. .once

   > C 

9. 在下面的双大括号标签中，（ ）是无效的表达式。 

   A. {{ number + 10 }}

   B. {{ str.toUpperCase() }}

   C. {{ sign ? '真' : '假' }}

   D. {{ if(sign) return 1}

   > D 

10. 在下列 Vue 指令中描述错误的是（ ）。 

    A. v-on 指令用于监听 DOM 事件

    B. v-show 指令用于判断是否显示或隐藏 DOM 元素

    C. v-html 指令可以更新元素的 innerHTML

    D. v-model 指令用于在表单控件元素上创建单向数据绑定

    > D 

11. 以下遍历并获取索引的正确方式（ ）。 

    A. <**tr v-for="(book,index) in books" :key= "index" **>

    B. <**tr v-for="book,index in books" :key= "index" **>

    C. <**tr v-for= "(index, book) in books" :key= "index"**>

    D. <**tr v-for="(index:book) in books" :key= "index"** >

    > A 

12. v-show 指令的特点是（ ）。 

    A. v-show 指令是通过修改元素的“display”CSS 属性让其显示或者隐藏

    B. v-show 指令是直接销毁和重建 DOM 达到让元素显示和隐藏的效果

    C. v-show 指令是操作 JavaScript 动态的把 DOM 进行隐藏或显示的效果

    D. 以上都不对

    > A 

13. 下列方法中，不是用于检测数组变化的变异方法的是（ ）。 

    A. push

    B. unshift

    C. splice

    D. filter

    > D 

14. 阻止默认事件的指令是（ ）。 

    A. .stop

    B. .self

    C. .prevent

    D. .capture

    > C 

15. 下列指令中，可以对表单元素进行双向数据绑定的是（ ）。 

    A. v-model

    B. v-on

    C. v-bind

    D. v-show

    > A 

16. 为 HTML 元素绑定属性需要使用（ ）指令。 

    A. v-if

    B. v-on

    C. v-model

    D. v-bind

    > D 

17. 如果要阻止浏览器的默认行为，需要使用（ ）事件修饰符。 

    A. .stop

    B. .prevent

    C. .self

    D. .once

    > B 

18. 可以看到下列在 Vue构造器中有一个data参数,关于data参数的描述正确的是（）。

    ```vue
    const app = Vue.createApp({
    
      data() {    
    
       return {
    
     }
    
    }
    
    }).mount('#app');
    ```

    A. data是一个对象

    B. data是一个函数

    C. data里面可以没有返回值

    D. data是一个属性

    > B 

19. 下列关于 v-if 和 v-show 的描述不正确的是。

    A. v-if与v-show都可以动态控制dom元素显示隐藏

    B. v-if不可以动态控制dom元素显示隐藏

    C. v-if显示隐藏是将dom元素整个添加或删除

    D. v-show隐藏则是为该元素添加css属性：display:none，dom元素还在

    > B 

20. 关于计算属性computed的说法，下面说法错误的是（）。 

    A. 计算属性在使用时不需要加(),直接写名称即可。

    B. 如果计算属性用到了data中的数据，当data数据发生变化时，就会立即重新计算这个计算属性的值

    C. computed 没有缓存的功能，每次访问计算属性会立即进行计算，返回结果。

    D. 计算属性在第一次使用时的结果会被缓存起来，直到属性中所依赖的data数据发生改变计算属性的结果才会重新求值

    > C 

21. 在computed中我们可以通过给计算属性添加（）方法以达到赋值效果。 

    A. setter 

    B. getter 

    C. set 

    D. get

    > C 

22. 以下关于computed和method的区别，说法不正确的是（）。

    A. computed具有响应式（双向数据绑定），以属性方式调用，如：this.reversedMessage。

    B. methods需以函数方式调用，如：this.reversedMessage()。

    C. method具有缓存功能，只要里面的数据不发生改变，就不会重新计算。

    D. computed比较适合对多个变量或者对象进行处理后返回一个结果值。

    > C 

23. 在 DOM 文档渲染完毕之后调用的钩子函数是（ ）。 

    A. beforeCreate

    B. created

    C. mounted

    D. unmounted

    > C 

24. 在 Vue.js 中，计算属性需要定义在（ ）选项中。 

    A. computed

    B. watch

    C. methods

    D. compute

    > A 

25. 下列关于 Vue 的优势的说法错误的是（ ） 

    A. 双向数据绑定

    B. 轻量级框架

    C. 增加代码的耦合度

    D. 实现组件化

    > C 

26. 下列关于生命周期钩子函数的说法错误的是（ ）。 

    A. beforeCreate 钩子在 Vue 实例开始初始化时调用

    B. created 钩子在实例创建之后进行调用

    C. mounted 钩子在 DOM 文档渲染完毕之后进行调用

    D. unmounted 钩子在实例被销毁之前进行调用

    > D 

27. Vue中实现数据双向绑定的是（ ）。 

    A. v-bind

    B. v-for

    C. v-model

    D. v-if

    > C 

28. 下面列出的钩子函数会在Vue实例销毁完成时执行的是（ ）。 

    A. updated

    B. unmounted

    C. created

    D. mounted

    > B 

29. Vue的生命周期，执行顺序正确的是：（） 

    A. beforeCreate→created→beforeMount→mounted→beforeUnmount→unmounted

    B. init→beforeMount→mounted→beforeUnmount→unmounted

    C. beforeMount→mounted→beforeCreate→created→beforeUnmount→unmounted

    D. init→beforeCreate→created→beforeUnmount→unmounted

    > A 

30. 哪一种数据绑定方法是不对的？ 

    A. {{if(x>1)x++;}}

    B. {{msg}}

    C. {{num+1}}

    D. {{sum=num+1}}

    > A 

31. Vue对象中可以使用（）属性来编写自定义函数？ 

    A. computed

    B. methods

    C. data

    D. mounted

    > B 

32. 完整的v-on语法<**a v-on:click="doSomething"></a**>可以缩写为（）。 

    A. <**a onclick　="doSomething"></a**>

    B. <**a :click="doSomething"></a**>   

    C. <**a @click="doSomething"></a**>

    D. <**a click="doSomething"></a**>

    > C 

33. 在Vue中如果想实现用户已经登录，浏览器显示“欢迎登录”；如果没有登录，浏览器就显示一个“登录”的链接，需要使用以下哪个指令？（） 

    A. v-on 

    B. v-if 

    C. v-for 

    D. v-else 

    > B 

34. 下列关于过渡的描述错误的是（ ）。 

    A. transition 组件只会把过渡效果应用到其包含的内容上，不会额外渲染 DOM 元素

    B. 自定义的过渡类名的优先级高于普通的类名

    C. 在默认行为中，元素的进入和离开是同时发生的

    D. 定义离开过渡的开始状态的 class 类名是 v-leave-to

    > D 

35. 在元素显示与隐藏的过渡中，用于定义元素离开过渡的结束状态的 class 类名是（）

    A. v-enter-from

    B. v-enter-active

    C. v-leave-to

    D. v-leave-active

    > C 

36. 下列关于Vue 3.x 为标签提供的过渡类名的说法，错误的是（）。 

    A. v-enter-from在元素被插入之前生效，在元素被插入之后的下一帧移除

    B. v-leave-from在离开过渡被触发时立刻生效，下一帧被移除

    C. v-enter-active可以控制进入过渡的不同的缓和曲线

    D. 如果name属性为my-name，那么my-就是在过渡中切换的类名的前缀

    > D 

37. 下列选项中关于多个元素过渡的说法，错误的是（）。 

    A. 当有相同标签名的元素切换时，需要通过key特性设置唯一的值来标记以让Vue区分它们

    B. 不相同元素之间可以使用v-if和v-else来进行过渡

    C. 组件的默认行为指定进入和离开同时发生

    D. 不可以给同一个元素的key特性设置不同的状态来代替v-if和v-else

    > D 

38. 在使用Vue过渡的时候需要使用下列哪个标签？（） 

    A. Animation  

    B. Animate 

    C. Transform 

    D. Transition

    > D 

39. Vue 3.x提供了 Transition 的封装组件，可以给任何元素和组件添加过渡动画，在进入/离开的过渡中，会有（）个 class 切换。 

    A. 5 

    B. 6

    C. 7

    D. 8

    > B 

40. 下列关于组件的描述错误的是（ ）。 

    A. 局部注册的组件只能在其父组件中使用，而无法在其它组件中使用

    B. 组件选项对象中的 data 和 Vue 实例选项对象中的 data 的赋值是不一样的

    C. 全局组件可以使用链式方法注册

    D. 全局组件可在所有实例中使用

    > B 

41. 下列关于组件 props 的描述错误的是（ ）。 

    A. props 是组件用来声明从父容器传递的数据的自定义属性

    B. 使用 props 传递的数据可以是数值和字符串类型，还可以是数组或对象类型

    C. 使用 props 验证的时候，props 接收的参数是一个数组

    D. 如果 props 传递的是一个对象或数组，那么它是按引用传递的

    > C 

42. 关于 Vue 组件之间的传值，以下说法错误的是（ ）。 

    A. 父组件给子组件传值使用 props

    B. 子组件给父组件传值使用$emit

    C. 非父子组件之间不能传值

    D. 一个组件从父组件接收的数据可以继续传递给子组件

    > C  

43. 子组件调用父组件的方法是（ ）。 

    A. this.emit

    B. this.$route.params

    C. this.$axios

    D. this.$emit

    > D 

44. Vue中如果希望组件能够被在它们第一次被创建的时候缓存下来，我们可以用一个（）元素将其动态组件包裹起来。

    A. <keep_alive> 

    B. <**keep-alive**> 

    C. <**keep-live**> 

    D. <keep_live>

    > B 

45. 如果想注册局部组件，Vue实例中接受的选项是（  ）。 

    A. directives 

    B. directive 

    C. component 

    D. components 

    > D 

46. 下列关于Vue的组件说法不正确的是（） 

    A. 不一定要写style

    B. template视图里面不可以写多个div容器

    C. 父组件给子组件传值需要定义props属性

    D. 子组件与父组件通信需定义$emit属性

    > B 

47. 关于下面代码中自定义组件的说法正确的是：（)

     ```html
    <script>
    const app=Vue.createApp({});
    app.component("MyComponent",{
    template:<p>自定义组件</p>
    });
    app.mount("#app");
    </script>
     ```

    A. MyComponent是组件名

    B. 使用<mycomponent></mycomponent>调用组件

    C. template下不可以有多个标签

    D. template下只能有一个根节点

    > A 

48. 使用下面全局注册组件正确的是（）。 

    A. Vue.methods("component-a",{/*....*/});

    B. Vue.props("component-a",{/*....*/});

    C. 

    const app=Vue.createApp({});

    app.components("component-a",{/*....*/});

    D. 

    const app=Vue.createApp({});

    app.component("component-a",{/*....*/});

    > D 

49. 下列选项中，（ ）是基于 Chrome V8 引擎的 JavaScript 运行环境，它可以让JavaScript运行在服务器端。

    A. npm.js

    B. jQuery.js

    C. vue.js

    D. Node.js

    > D 

50. 下列选项中，用来为Vue CLI安装模块时的正确命令是（ ）。 

    A. npm install modulename

    B. node.js install modulename

    C. node install modulename

    D. npm I modulename

    > A 

51. 下列关于路由的描述错误的是（ ）。 

    A. 通过组件的 to 属性可以设置目标地址，从而切换不同的 HTML 内容

    B. 一个被渲染的组件的模板中可以包含嵌套的

    C. 使用 router 的 to()方法也可以实现导航的功能

    D. 如果为要访问的路径设置了重定向规则，则访问该路径时会被重定向到指定的路径

    > C 

52. 以下获取动态路由{ path: '/user/:id' }中 id 的值正确的是（ ）。 

    A. this.$route.params.id

    B. this.route.params.id

    C. this.$router.params.id

    D. this.router.params.id

    > A 

53. 以下选项中不可以进行路由跳转的是（ ）。 

    A. push()方法

    B. replace()方法

    C. router-link 组件

    D. jump()方法

    > D 

54. 下列关于 query 方式传参的说法，正确的是（ ） 

    A. query 方式传递的参数会在地址栏展示

    B. 在页面跳转的时候，不能在地址栏看到请求参数

    C. 在目标页面中使用“this.route.query.参数名”来获取参数

    D. 在目标页面中使用“this.$route.params.参数名”来获取参数

    > A 

55. 在 Vuex 的组成部分中，下列描述错误的是（ ）。 

    A. state 用于存储项目中需要共享的数据或状态

    B. getters 可以从 state 中派生出一些状态

    C. mutations 是 Vuex 中唯一修改 state 的方式，支持异步操作

    D. actions 可以通过提交 mutations 中的方法来改变状态

    > C 

56. 下列不属于 Vuex 的组成部分的是（ ）。 

    A. getters

    B. setters

    C. mutations

    D. actions

    > B 

57. 下面关于 Vuex 核心模块的说法，错误的是（ ）。 

    A. Vue组件可以直接修改Vuex 中 state的状态

    B. Vuex配置对象中，actions选项是异步的

    C. Vuex 配置对象中，mutations选项是同步的

    D. Vuex 中，通过 commit()方法完成 mutations 提交

    > A 

58. 关于路由模式说法错误的是（）。 

    A. vue-router 有两种模式，history 和 hash 模式

    B. history 通过 H5 提供的 API history.pushState 和 history.replaceState 实现跳转且不刷新页面

    C. hash 模式是通过 onchange 事件，监听 url 的修改

    D. history 模式需要后端进行配合

    > C 

59. 关于 Vue-CLI 说法错误的是（）。 

    A. Vue CLI 是一个基于 Vue.js 进行快速开发的完整系统

    B. cli(@vue/cli) 是一个全局安装的 npm 包，提供了终端里的 Vue 命令

    C. CLI目前还不能提供图形化界面管理所有的项目

    D. CLI服务是构建于 webpack 和 webpack-dev-server 之上

    > C 

60. 使用 axios 发送请求时，用于处理请求失败的回调函数的方法是（）。 

    A. then()

    B. get()

    C. post()

    D. catch()

    > D 

61. 在Vue3组合式API中，用于定义组件的自定义属性可以使用（）。

    A. defineProps

    B. defineEmits

    C. defineExpose

    D. defineAsyncComponent

    > A 

62. 在Vue中，依赖函数provide和注入函数inject的作用是什么？ 

    A. 用来在组件树中传递数据和方法的

    B. 用来创建全局变量和全局方法的

    C. 用来创建局部变量和局部方法的

    D. 用来在组件之间进行通信的

    > A 



# 判断题

1. Vue是一套构建用户界面的渐进式框架，Vue的核心只关注视图层。

   > 对 

2. 在Vue中beforeUnmount与unmounted生命周期函数执行后，都可以获取到Vue实例。 

   > 对 

3. Vue 3.x中data函数中的数据具有响应特性。

   > 对 

4. Vue.js和React一样，是数据的单向绑定。

   > 错 

5. 因为Vue.js只需关心数据，更新DOM由Vue完成，所以开发者可以把更多的精力放在编写业务逻辑上。 

   > 对 

6. Vue的created生命周期表示已完成数据绑定和事件配置，此时尚未生成DOM。 

   > 对 

7. 给过渡元素添加v-bind:css="true"，Vue会跳过CSS的检测。 

   > 错 

8. 在@before-enter钩子函数中可以设置元素开始动画之前的起始样式。

   > 对 

9. Vue开发提出了组件化开发思想，每个组件都是一个孤立的单元。 

   > 对 

10. Vue提供的全局API接口component()，不能用来注册组件。（ ） 

    > 错 

11. 在组件中，可以随时修改由Props传递过来的数据 

    > 错 

12. 组件定义完成后，就可以直接使用 

    > 错 

13. Vue完全能够为复杂的单页应用提供驱动。 

    > 对 

14. 在Vue3的组合式API中，watch方法会在组件加载时自动执行1次。 

    > 错 

15. axios 是一个基于 Promise 的 HTTP 库，可以用于发送 HTTP 请求。

    > 对 

16. Vue CLI的SPA项目中，组件的模板中只能包含1个router-view组件。 

    > 错 

17. 在 Vuex 中，actions 用于处理异步操作和提交 mutations。 

    > 对 

18. Vuex 可以用于管理 Vue.js 应用中的单个组件的状态。

    > 错 

19. 在 Vuex 中，可以使用 getters 修改 state 中的数据。 

    > 错 

20. 在 Vue-Router 中，可以通过路由参数来传递数据，但是不能通过路由查询参数来传递数据。

    > 错 

# 填空题

1. 使用 watch 选项监听对象内部值的变化，可以在监听属性的选项参数中设置（ ）为true。 

   > deep

2. Vue.js 为 v-on 指令提供的事件修饰符中，使用（ ）修饰符可以阻止事件冒泡。 

   > stop

3. v-on 指令的简写形式是在事件名称前添加符号（ ） 

   > @

4. 在 DOM 中输出真正的 HTML 内容需要使用（ ）指令。 

   > v-html

5. 在 Vue.js 中，指令是带有（ ）前缀的特殊属性。 

   > v-

6. 当选中某个单选按钮时，v-model绑定的属性值会被赋值为该单选按钮的（ ）属性值。 

   > value

7. 对元素的 class 属性进行绑定时，绑定的数据可以是对象或（ ）。 

   > 数组

8. 对元素样式的绑定就是对元素的 class 属性或（ ）属性进行绑定。 

   > style

9. 如果有多个复选框，应用 v-model 绑定的是一个（ ）。 

   > 数组

10. MVVM 主要包含 3 个部分，分别是 Model、View 和（ ）。 

    > ViewModel

11. Vue 初始数据在实例对象的（ ）函数中进行定义。 

    > data();data（）

12. 每个Vue 3.x 应用都是通过_______函数创建一个新的应用实例。 

    > createApp

13. Vue 3.x 初始数据是在实例对象的_______函数中进行定义。 

    > data；data()

14. Vue 3.x 为标签内部的元素提供了 v-leave-from、v-leave-active、（ ）3 个离开的过渡的类。 

    > v-leave-to

15. 实现列表过渡需要使用（ ）组件。 

    > <transition-group>；transition-group；TransitionGroup

16. 在多元素过渡中，当有相同标签名的多个元素进行切换时，需要通过（ ）属性为元素设置唯一的值。

    > key

17. Vue提供了内置的过渡封装组件是_______。

    > transition；Transition

18. 在Vue中封装的过渡组件中使用_______属性可以重置过渡中切换类名的前缀。 

    > name

19. 通过设置过渡组件的_______属性可以实现节点在初始渲染的过渡。

    > appear

20. _____的类名优先级要高于普通的类名。 

    > 自定义过渡

21. Vue.js 提供了两种注册组件的方式，分别是全局注册和（ ）。 

    > 局部注册

22. 在使用动态组件时，需要将组件动态绑定到元素的（ ）属性， 根据该属性的值来判断使用哪个组件。

    > is

23. 插槽可以使用（ ）属性来配置如何分发内容，多个 slot 可以有不同的名字。 

    > name

24. 子组件给父组件传递数据通过（ ）事件触发的方式实现，父组件使用 v-on/@自定义事件进行监听即可。 

    > $emit

25. 父组件传递数据到子组件使用（ ）选项，并且这传递是单向的，只能由父组 件传到子组件。 

    > props

26. Vue中页面结构以_______形式存在。

    > 组件

27. 以下代码运行后，在界面上显示的文字为（ ）。

    ```html
    <div id="app">
             <my-button>{{value}}</my-button>
          </div>
          <script>
             var app=Vue.createApp({
               data(){
                 return {
                   value:"登录"
                 }
               }
             });
             app.component("my-button",{
               template:`<span><slot>注册</slot></span>`
             });
             app.mount("#app");
            </script>
    ```

    > 登录

28. Vue.js框架的单文件组件是以（ ）后缀命名的文件格式。 

    > .vue

29. Vue-router 的作用是将每个路径映射到对应的组件，并通过（ ）进行组件之间的切换。 

    > 路由

30. 通过一个名称来标识一个路由的方式称为（ ）。 

    > 命名路由

31. 通过路由实现组件之间的切换需要使用（ ）组件。 

    > <router-link>

32. 配置嵌套路由，需要在 Vue-Router 实例中使用（ ）参数进行配置。 

    > children

33. 除了使用创建标签可以定义导航链接之外，还可以使用 router的（ ）方法实现导航的功能。 

    > push()；replace()

34. 如果没有为 router-view 设置名称，那么它的名称默认为（ ）。 

    > default

35. 要链接到一个命名路由，可以给 router-link 的（ ）属性传一个对象。 

    > to

36. hash 模式路由，地址栏 URL 中会自带（ ）符号。 

    > #

37. 由于 Vuex 的状态存储是响应式的，从 store 实例中读取状态最简单的方法就是在（ ）中返回某个状态。 

    > 计算属性

38. Vuex 实例对象中组件状态通过（ ）改变。 

    > mutations

39. Vuex 中创建动态模块提供的方法是（ ）。 

    > registerModule()

    ```vue
    //使用示例：
    
    import { createStore } from 'vuex'
    
    const store = createStore({....})
    
    // 注册一个新的模块store.registerModule('myModule', 
    
    {  
    
     state: {   
    
       message: 'Hello!' },  
    
     mutations: {   
    
      updateMessage(state, newMessage) {    state.message = newMessage   }  } })
    ```

    

40. 在组件中访问定义的 getter 可以使用简化的写法，即通过辅助函数（ ）将 store中的 getter 映射到局部计算属性。 

    > mapGetters

41. 使用axios发送请求时,用于处理请求成功的回调函数的方法是（）。 

    > then；then()

42. 在编写Vue单文件组件时，如果希望一些样式只作用于这一个组件，需要在style标签中加上_________属性。 

    > scoped

43. Vue 3中使用组合式 API 的编译时语法糖，需要要<**script**>中加入属性____________。 

    > setup

# 简答题

1. 计算属性和监听器的区别

   > 计算属性的get必须有return，而监听器可有可无；
   >
   > 计算属性具有缓存效果，而监听器无；
   >
   > 计算属性可以自定义名称，而监听器只能监听和data或computed里的名称相同的数据；
   >
   > 计算属性适用于复杂运算，而监听器适合一些消耗功能，例如Ajax请求

2. 请简单介绍Vue数据绑定内置指令内容有那些

   > v-model：双向数据绑定;
   >
   > v-on：监听事件;
   >
   > v-bind：单向数据绑定;
   >
   > v-text：插入文本内容;
   >
   > v-html：插入包含HTML的内容
   >
   > v-for：列表渲染
   >
   > v-if：条件渲染
   >
   > v-show：显示隐藏

3. 请简述MVVM模式

   > MVVM全称是Model-View-ViewModel
   >
   > Model代表整个Web项目所需要的数据模型， Model含有大量信息，但它并不具有任何行为逻辑，它只是数据，因而它不会影响浏览器如何展示数据。
   >
   > View是具有主动性的，因为它包括了一些数据绑定、事件和行为，这些都会直接影响Model和ViewMode的。   
   >
   > ViewModel：MVVM中的VM它主要负责用一定的业务逻辑对数据进行改变或转换，它也负责将Model的变化反应到View上。

4. 请简述Vue3.x中实现JavaScript过渡的钩子函数包括哪些

   > @before-enter，当进入过渡完成前调用
   >
   > @enter,当进入过渡完成时调用
   >
   > @after-enter,当进入过渡完成后调用
   >
   > @before-leave,在离开过渡开始前调用
   >
   > @leave,在离开过渡开始时调用
   >
   > @after-leave,在离开过渡开始后调用

5. 请简述Vue3.x中Transition组件的6个内置的过渡名

   > 进入阶段（enter）： 
   >
   >   v-enter-from: 在元素被插入之前生效，在元素被插入之后的下一帧移除 
   >
   >   v-enter-active: 在整个进入过渡的阶段中应用，在元素被插入之前生效，在过渡动画完成之后移除 
   >
   >    v-enter-to: 在元素被插入之后下一帧生效（与此同时v-enter被移除），在过渡动画完成之后移除 
   >
   > 离开阶段（leave）： 
   >
   >    v-leave-from：在离开过渡被触发时立刻生效，下一帧被移除 
   >
   >    v-leave-active：在整个离开过渡的阶段中应用，在离开过渡被触发时立刻生效，在过渡完成之后移除 
   >
   >    v-leave-to：在离开过渡被触发之后下一帧生效（与此同时v-leave被移除），在过渡动画完成之后移除

6. 请简述Vue.js3.x提供Props验证方式有哪几种

   > 基础类型检测、
   >
   > 多种类型检测、
   >
   > 参数必须的检测、
   >
   > 参数具有默认值的检测、
   >
   > 自定义验证函数的检测

7. 请简述Vuex配置对象中的主要内容有哪些

   > state：包含应用程序状态的对象。
   >
   > mutations：包含用于修改 state 的函数。
   >
   > actions：包含用于触发 mutations 的函数。
   >
   > getters：包含从 state 中派生出一些状态的函数。
   >
   > modules：允许将 store 拆分为更小的模块，每个模块都可以具有自己的 state、mutations、actions 和 getters。

8. 动态路由与普通路由有什么区别

   > 动态路由和普通路由最大的区别在于是否包含参数。普通路由是指固定的路由路径，而动态路由则是包含参数的路由路径。在Vue.js中，需要使用不同的方式来定义和获取这两种类型的路由。

# 知识点总结

