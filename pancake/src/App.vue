<template>
  <div id="app">
    <img src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Product title="Socks" v-bind:product="{price: '7.33', description: 'Socks for sale!', img:'http://baconmockup.com/300/300'}"/>
    <Product title="V-neck Sweaters" v-bind:product="{price: '15.89', description: 'Argyle and fuzzy sweaters for sale!', img:'http://baconmockup.com/300/200'}"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Product from './components/Product.vue'
export default {
  name: 'app',
  components: {
    HelloWorld, Product
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
