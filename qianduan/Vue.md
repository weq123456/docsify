#                                                Vue

### CSS 预处理器  

- SASS:基于Ruby,通过服务器处理，功能强大，解析效率高，需要学习Ruby语言，上手难度高于LESS
- LESS:基于NodeJS,通过客户端处理，使用简单，功能比SASS简单，解析xiaolv也低于SASS，但在实际开发中足够了，所以我们后台人员如果需要的话，建议使用LESS

### javaScript框架:

1.    jQuery: 大家都熟知的JavaScript，优点是简化了DOM操作，缺点是DOM操作台频繁，影响前端性能，在前端眼里使用它仅仅是为了兼容IE6,7,8
2. Angular:Google 收购的前端框架，又一群java程序员开发，其特点是将后台的MVC模式搬到了前端并增加了模块化开发的理念，与微软合作，采用TypeScript语法开发；对后台程序员友好，对前端程序不太友好；做大的缺点是版本迭代不合理（如：1代->2代，除了名字，基本就是两个东西；截止发表博客时已推出了Angular6）
3. React: Facebook 出品，一款高性能的JS前端框架：特点是提出了新开年【虚拟DOM】用于减少真是DOM操作，在内存中模拟DOM操作，有效的提升了前端渲染效率；缺点是使用复杂，因为需要额外学习一门【JSX】语言
4. Vue：一款渐进式JavaScript框架，所谓渐进式就是逐步实现新特性的意思，如实现模块化开发，路由，状态管理扥更新特性，其特点是综合了Angular(模块化)和React(虚拟DOM)的优点。
5. Axios：前端通信框架，因为VUe的便捷很明确，就是为了处理DOM，所以并不具备通信能力，此时就需要额外使用一个通信框架与服务器交互；当然也可以直接选择使用jQuery提供的AJAX通信功能。

### UI框架

- Ant-Design: 阿里巴巴出品，基于React的UI框架

- ElementUI , iview,   ice：饿了么出品，基于Vue的UI框架

- BootStrap:  Twitter推出的一个用于前端开发的开源工具包

- AmazeUI：又叫“妹子UI”,一款HTML5跨屏前端框架


### JavaScript 构建工具

-   Babel: JS编译工具，主要用于浏览器不支持的ES新特性，比如用于编译TypeScript
- WebPack: 模块打包器，主要作用是打包，压缩，合并及按序加载

### Vue.js

- ​    iview是一个强大的基于Vue的UI库，有很多使用的基础组件比elementui的组件更丰富，主要服务于ps界面的中后台产品。使用单文件的Vue组件化开发模式基于npm+webpack+babel开发，支持ES2015高质量，功能丰富友好的API,自由灵活的使用空间。iview-admin 属于前端主流框架，选型时可以考虑使用，主要特点是移动端支持较多。
- Element 是饿了么前端开源维护的VueUI组件库，组件齐全，基本涵盖后台所需的所有组件，文档讲解详细，例子也很丰富。主要用于开发ps端的页面，是一个质量比较高的VueUI组件库。 vue-element-admin 属于前端主流框架，选型时可 考虑使用，主要特点是桌面端支持较多
- ICE 飞冰是阿里巴巴团队基于React/Angular/Vue的中后台应用解决方案，在阿里巴巴内部，已经有了270对个来自几乎所有BU的项目在使用。飞冰包含了一条从设计端到开发端的完整链路，帮助用户快速搭建属于自己的中后台应用。主要组件还是以React为主，截止2019年02月17日更新博客前对Vue的支持还不太完善，目前尚处于观望阶段。
- VantUI 是有赞前端团队基于有赞统一的规范实现的Vue组件库，提供了一整套UI基础组件和业务组件。通过Vant,可以快速搭建出风格统一的页面，提升开发效率。
- at-ui 是一款基于 Vue 2.x的前端UI组件库，主要用于快速开发ps网站产品。它提供了一套npm+webpack+babel前端开发工作流程，css样式独立，及时采用不同的框架实现都能宝石统一的UI风格。
- Cube-ui是滴滴团队开发的基于Vue.js实现的精致移动端组件库。支持按需引入和后编译，轻量灵活扩展性抢，可以方便地基于现有组件实现二次开发
- Flutter 是谷歌的移动端 UI框架，可在极短的时间内构建 Android 和 IOS 上高质量的原生级应用。Flutter 可与现有代码一起工作，它被世界各地的开发者和组织使用，并且Flutter 是免费和开源的 Google出品，主要特点是快速构建原生APP应用程序，如做混合应用该框架为必选框架
- Ionic既是一个css框架也是一个Javascript UI 库，Ionic是目前最有潜力的一款HTML5手机应用开发框架。通过SASS构建应用程序，它提供了很多UI组件来帮助开发者开发强大的应用。它使用JavaScript MVVM框架和AngularJS/Vue来增强应用。提供数据的双向绑定，使用它成为web和移动开发者的共同选择。
- 微信小程序  mpvue 是美团开发的一个使用 Vue.js开发小程序的前端框架，目前支持微信小程序。百度智能小程序，头条小程序和支付包小程序。框架基于 Vue.js，修改了的运行时框架runtime 和 代码编译器 compiler 实现，使其运行在小程序环境中，从而为小程序开发引入了 Vue.js 开发体验。完备的Vue开发体验，并且支持多平台的小程序开发，推荐使用。
- WeUI 是一套同微信原生视觉体验一致的鸡翅样式库，由微信官方设计团队为微信内网页和微信小程序量身设计，令用户的使用感知更加统一。包含button,cell，dialog.toast.article.icon等格式元素。好                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    



###  Vue开发

​      Vue开发都是基于NodeJS,实际开发采用Vue-cli脚手架开发，vue-router路由，vuex做状态管理，VueUI，界面我们一般使用ElementUI(饿了么出品)，或者ICI阿里巴巴出品来快速搭建前端项目

​    官网：

- https://element.eleme.cn
- https://ice.work/

### Vue语法

- v-bind  绑定数据  css的样式、对象、数组、number 类型、bool类型 

  ```java
  <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
  <div id="app2">
      <span v-bind:title="test1">
          鼠标悬停几秒钟查看此处动态绑定的提示信息！
      </span>
  
  </div>
    var app3 = new Vue({
          el: '#app2',
          data: {
              test1: '页面加载于 '+new Date().toLocaleString()
          }
      })
  ```

  

- v-model  数据双向绑定

  ```java
  <div id="app7">
     <select v-model="selected" >
         <option value="" disabled >请选择</option>
         <option >A</option>
         <option >B</option>
         <option >C</option>
     </select>
      <p>{{selected}}</p>
  </div>
         var vm = new Vue({
          el: '#app7',
          data: {
              selected: '34234'
          }
      })
      <div id="app6">
      <input type="radio" name="sex" value="男" v-model="text" > 男
      <input type="radio" name="sex" value="女" v-model="text"> 女
      <p>选中了谁：{{text}}</p>
  </div>
    var vm1 = new Vue({
          el: '#app6',
          data: {
              text: '男'
          }
      })
  ```

  

- > v-for = “(item,index) in list”

- > v-if=“true”   v-else

- 组件  

   ```html
   <div id="app">
       <todo-item v-for="item in groceryList" v-bind:todo="item" v-bind:key="item.id">
       </todo-item>
   </div>
   Vue.component('todo-item', 
                  //传递参数
                 {    props: ['todo'],    
                  template: '<li>{{todo.id}}</li>' //定义模板
                 })
   
    var app = new Vue({
       el: '#app',
       data: {
           groceryList: [
               { id: 0, text: '蔬菜' },
               { id: 1, text: '奶酪' },
               { id: 2, text: '随便其它什么人吃的东西' }
           ]
       }
   });
   
   
   
   
   ```

- axios 网络交互通信

     ```java
     script src="https://unpkg.com/axios/dist/axios.min.js"></script>
     data(){
              return{
                  info:{
                      name: null,
                      url: null
                  }
              }
         },
      mounted(){
           axios.get('data.json').then(response=>(this.info=response.data))
     
       }
     ```



- 计算属性

  ```java
   <p>{{computedTime}}</p>
    <p>{{computedTime1()}}</p>
  
  methods: {
              computedTime1: function () {
                  return Date.now();
              }
          },
  
          //虚拟dom 内存中运行
          computed: {
              reversedMessage: function () {
                  return this.message.split('').reverse().join('');
              },
              computedTime: function () {
                  return Date.now();
              }
          }
  ```

  

-   插槽slot  自定义事件remove

    ```java
    <div>
    <todo>
        <todo-title slot="todo-title" :title="title"></todo-title>
        <todo-list slot="todo-list" v-for="(item,index) in novelList"  :item="item" :index="index" @remove="removeItem(index)" ></todo-list>
    </todo>
    
    </div>
    
    <script>
        Vue.component('todo',{
            template: '<div>\
                           <slot name="todo-title"></slot>\
                           <ul>\
                             <slot name="todo-list"></slot>\
                            </ul>\
                        </div>\
                '
        });
    <script>
        Vue.component('todo',{
            template: '<div>\
                           <slot name="todo-title"></slot>\
                           <ul>\
                             <slot name="todo-list"></slot>\
                            </ul>\
                        </div>\
                '
        });
    
    Vue.component('todo-title',{
        props: ['title'],
        template: '<div>{{title}}</div>'
    });
    Vue.component('todo-list',{
        props: ['item','index'],
        //只能绑定当前组件的方法
        template: '<li>{{index}}---{{item}}--- <button @click="remove">删除</button></li>',
        methods: {
            remove: function (index){
                this.$emit('remove',index);
            }
        }
    
    });
    
    var vm = new Vue({
        el: "#app",
        data:{
            title: '小说系列',
            novelList: ['斗罗大陆','吞噬星空','刺探小说家']
        },
        methods:{
    
            removeItem:function (index){
                console.log("删除了"+this.novelList[index]+"ok");
                this.novelList.splice(index,1)
            }
        }
    })
    ```

### Webpack

  webPack是一款模块加载器兼打包工具，它能把各种资源，如JS，JSX.ES6,SASS,LESS.图片等都作为模块来处理使用

### 创建工程命令

```java
-创建项目名
 vue init webpack hello-vue
- 进入工程目录     
    cd hello-vue
- 安装 vue-router
    npm install vue-router --save-dev
 安装 element-ui -s
    npm i element-ui -s
 安装依赖
    npm install
    
 安装 SASS加载器
    cnpm install sass-loader node-sass --save-dev
 启动测试
    npm run dev
    
```



#### npm 命令解释：

-  npm install moduleName: 安装模块到项目目录下
- npm install -g moduleName: -g  的意思是将模块安装到全局，具体安装到磁盘那个位置，要看 npm config prefix 的位置
- npm install -save moduleName: —save的意思是将模块安装到项目目录下，并在package 文件的dependencies 节点写入依赖，-s为命令的缩写。
- npm install -save-dev  moduleName: --save-dev的意思是将模块安装到项目目录下，并在package文件的devDependencies节点写入依赖， -D为该命令的缩写。

