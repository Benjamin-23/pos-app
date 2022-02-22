<template>
<form action="">
    <div class="shop-name">
        <label for="shopName">Shop Name</label>
        <input type="text" id="name" v-model="shopValue.name">
    </div>
</form>

</template>

<script>
export default {
    name:'shopOrg',
    data() {
      return{
          shopValue: {
              id:'',
              name:'',
              directors:'',
              headquarters:'',
              service:'',
              networth:'',
              shopStatus:''  
              
          }
      }  
    },
}
</script>