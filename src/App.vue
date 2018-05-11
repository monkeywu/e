<template>
  <div>
    <div class="menu">
      <router-link to="/about">about</router-link>
      <router-link to="/product">product</router-link>
    </div>
    <router-view></router-view>
  </div>
</template>

<script>
  import VueRouter from 'vue-router'
  import Product from './product.vue'
  import About from './about.vue'

  export default {
    router : new VueRouter({
      routes:[
        {path:'/about',component:About},
        {path:'/product',component:Product}
      ]
    })
  }
</script>
