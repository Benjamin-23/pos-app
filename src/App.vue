<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Pos-trial"/>
  <sales msg = " Today's Sales"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import sales from './components/sales.vue'
import event from './components/event.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    sales,
    event
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
