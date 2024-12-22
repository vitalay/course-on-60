<script>
export default {
  name: 'App',
   data() {
    return {
			 items: [0, 1, -2, 3, -4, 5],  
   


     }
   },

};
</script>

<template>

<ul>
	<template v-for="item in items">
		<li v-if="item >= 0">
			{{ item }}
		</li>
	</template>
</ul>


</template>


<style scoped>
table {
  border: 1px solid black;
}
td {
	border: 1px solid black;
}
</style>


