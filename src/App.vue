<script>
export default {
  name: 'App',
   data() {
    return {
      age: 26,
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
    <p v-if="age < 18">подросток</p>
	<p v-else-if="age >= 18 && age <= 25">взрослый</p>
  <p v-else>старик</p>
  </div>
</template>


<style scoped>
* {
  margin: 0;
  padding: 0; 

}
</style>


