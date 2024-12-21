<script>
export default {
   data() {
    return {
      visible1: true,
      visible2: true,
      visible3: true,
     }
   },
   methods: {
     toggle1() {
       this.visible1 = !this.visible1
     },
     toggle2() {
       this.visible2 = !this.visible2
     },
     toggle3() {
       this.visible3 = !this.visible3
     }
       
   },
   computed: {
    
   }

};
</script>

<template>
  <div>
    <button @click="toggle1">{{ visible1 ? 'hide' : 'one' }}</button> 
    <button @click="toggle2">{{ visible2 ? 'hide' : 'one' }}</button>
    <button @click="toggle3">{{ visible3 ? 'hide' : 'one' }}</button>
  
<p v-if="visible1">Hello World11</p>
<p v-if="visible2">Hello World22</p>
<p v-if="visible3">Hello World33</p>

  </div>
</template>


<style scoped>

</style>


