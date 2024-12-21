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
    <div v-show="isAuth">
		<p>one</p>
		<p>two</p>
		<p>three</p>
	</div>
  </div>
</template>


<style scoped>
* {
  margin: 0;
  padding: 0; 

}
</style>


