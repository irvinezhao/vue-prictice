MVVM 可以拆分成：View --- ViewModel --- Model 三部分


用 Vue.component(tagName, options) 注册了一个名字叫 card 的组件，这样，在需要复用这个组件的地方，我们只需要使用 <card></card> 就可以了。实际开发中，组件比这个复杂得多，越复杂，封装后的便利性越高。



视图 view 部分：


  <div id="app"></div>



视图（html 部分）上我们有一个 id 为”app” 的 div 元素。




  let vm = new Vue({
    //挂载元素
  el:'#app',
    //实例vm的数据
  data:{
        name: "张三",
        age :  21
    }
  });




  Vue 把整个生命周期划分为创建、挂载、更新、销毁等阶段
