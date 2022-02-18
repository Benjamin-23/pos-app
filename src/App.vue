<template>
  <img alt="pos logo" src="./assets/pos.jpg">
  <HelloWorld msg="Welcome to Pos-trial"/>
  <product productName="Product"/>

</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Product from './components/Product.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Product
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
