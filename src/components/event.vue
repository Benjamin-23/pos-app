<script>
export default {
    name:'event',
     data() {
         return{
             count:0
         }
     }
}
  
</script>
<template>
    <button @click="count++">Add</button>
    <p>count is:{{count}}</p>
</template>