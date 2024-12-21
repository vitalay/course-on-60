<script>
export default {
   data() {
     return {
      cost: 15,
      amount: 10
     }
   },
   methods: {
   


   },
   computed: {
    
     price: function(){
      return this.cost * this.amount + '$'
     },
   

   }

};
</script>

<template>
  <div>
   
    
<p>{{ price }}</p>
<button @click="cost++">сумма</button>
  </div>
</template>


<style scoped>

</style>


