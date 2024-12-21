<script>
export default {
  name: 'App',
   data() {
    return {
     
        items: [1, 2, 3],

     }
   },

};
</script>

<template>
<ul >
  
  <li v-for="item in items">{{ item }}</li>

  <li class="divider"></li>
</ul>
</template>


<style scoped>

</style>


