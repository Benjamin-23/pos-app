<script>
export default {
        name:'product',
        props: {
            productName:String
    
        },
 
    data() {
        return {
            formValue: {
                id:'1',
                name:'',
                description:'',
                category:'',
                buyingPrice:'',
                sellingPrice:'',
                
                }
        }
    },
    methods:{
        submitForm(event){
            event.enter()
            console.log(this.formValue)
        }
    }
}

  
</script>
<template>
    <form @submit="submitValues">
        <div>
            <pre>
               {{JSON.stringify(formValue, null,2)}}
            </pre>
        </div>
        <div>
            <h1>{{productName}}</h1>
            <label for="itemName">Product Name</label>
            <input type="text" id="name" v-model="formValue.name">
        </div>  

         <div>
            <label for="itemDescription">Description</label>
          <textarea name="description" id="description" v-model="formValue.description" cols="20" rows="5"></textarea>
        </div>
        <div>
                <label for="category">Product Category</label>
               <select name="category" id="category" v-model="formValue.category">
                   <option id="foodStuff" value="foodStuff">Food Stuff</option>
                   <Option id="clothes" value="clothes">Clothes</Option>
                   <option id="paints "   value="paint">paints</option>
               </select>
        </div>
        <div>
            <label for="buyingPrice">Buying price</label>  
            <input type="number" id="buyingPrice" v-model="formValue.buyingPrice">
        </div>
        <div>
            <label for="sellingPrice">Selling price</label>  
            <input type="number" id="sellingPrice" v-model="formValue.sellingPrice">
        </div>
        <div>
            <button>Submit</button>
        </div>

    </form>
</template>

<style>
form{
    display: inline-block;
    margin: 20px 0 0 40px;
}
label{
    margin:auto;
    display: grid;
}
input, textarea{
    margin-top: 7px;
}
</style>