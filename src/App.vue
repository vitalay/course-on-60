<script>
export default {
   data() {
     return {
       text: 'xxx'
     }
   },
   methods: {
      change () {
         this.text = 'yyy'
      },
      change2 () {
         this.text = 'zzz1111'
      }


   }
};
</script>

<template>
  <div>
   
   
    <button @click="change">Нажми</button>
    <button @click="change2">Нажми2</button> 
    <p>{{ text }}</p>
  </div>
</template>


<style scoped>

</style>


