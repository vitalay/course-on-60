<script>
export default {
  name: 'App',
   data() {
    return {
      isAuth: true
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
    <button @click="isAuth = !isAuth">Скрыть</button>
    <template v-if="isAuth">
		<p>one</p>
		<p>two</p>
		<p>three</p>
	</template>
  </div>
</template>


<style scoped>
* {
  margin: 0;
  padding: 0; 

}
</style>


