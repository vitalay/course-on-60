<script>
export default {
   data() {
    return {
      visible: true,
   
     }
   },
   methods: {
       
   },
   computed: {
    
   }

};
</script>

<template>
  <div>
    <button @click="visible = true" v-if="!visible">показать</button>
    <button @click="visible = false" v-if="visible">скрыть</button>
<p v-if="visible">Hello World</p>

  </div>
</template>


<style scoped>

</style>


