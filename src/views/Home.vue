<template>
<!--html-->
  <div id="nav">
    <h1>Enter Amount</h1>
    <!-- <h1>{{name}}</h1>
    <h1>{{age}}</h1>
    <h1>{{address}}</h1>
    <h2>{{number1+number2}}</h2> -->

    <!--form data binding-->
    <input type="number" v-model="amount">
    <!-- <input type="number" v-model.number="number2"> -->
    <button @click="Increase_Qua">Increse_qua</button>

    amount: {{amount}}
    Quantity: {{quantity}}
    Subtot: {{Subtot}}

    <button @click="Clear">Clear</button>
  
  </div>
  <!--html-->
</template>

<script>
export default {
  data(){
    return{
      // name:"",
      // age:23,
      // address:"Kegalle",
      // number1:0,
      // number2:0,
    
      amount:0,
      quantity:0,
      Subtot:0,
      quantityCount:0

    }
  },
  components: {
  
  },

methods:{
  Increase_Qua(){
    
    this.quantity++
    this.Subtot = this.quantity * this.amount


    }
     
  }
}
</script>


<style>

</style>
