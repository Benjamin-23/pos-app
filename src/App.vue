<template>
  <img alt="pos logo" src="./assets/pos.jpg">
  <HelloWorld msg="Welcome to Pos-trial"/>
  <products></products>
  <shopOrg/>
  <shopOrg/>

</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import products from './components/products.vue'
import shopOrg from './components/shopOrg.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    products,
    shopOrg
  },

}
</script>

<style>
#app {
background-color: rgb(218, 253, 241);
  margin-top: 10px;
}
img{
  height: 256px;
  width: 256px;
}

</style>
