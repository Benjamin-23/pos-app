<script>
let id = 0
    export default{
        name:'sales',
        props: {
            msg:String
        },
         data() {
             return {
                 newSale:'',
                 sales:[
                     {id: id++, text: 'kiwi'},
                     {id: id++, text: 'soap'}
                 ]
             }
         },
         methods:{
             addSale(){
                 this.sales.push({id:id++, text:this.newSale})
                 this.newSale =''
             },
             removeSale(sale) {
                 this.sales = this.sales.filter((t) => t !== sale)
             }
         }
    }
</script>



<template>
<div class="sales">
    <h2>{{msg}}</h2>
    <input v-model="newSale" @keyup.enter="addSale">
    <button @click="addSale">Add sale</button >
    <ul>
        <li v-for="sale in sales" :key="sale.id">
            {{sale.text}}
            <button @click="removeSale(sale)"> Remove</button>
        </li>
    </ul>
</div>
</template>
  

