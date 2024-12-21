<script>
export default {
  name: 'App',
   data() {
    return {
      obj: {
	user1: '100$',
	user2: '200$',
	user3: '300$',
}
     }
   },

};
</script>

<template>

  <ul>
    <li v-for="(elem, key, index) in obj" >{{ key }} - {{ elem }} - {{ index + 1 }}</li>
  </ul>


  
</template>


<style scoped>

</style>


