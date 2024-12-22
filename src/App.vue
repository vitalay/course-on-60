<script>
export default {
  name: 'App',
   data() {
    return {
			// items: [1, -2, 3, -4, 5],  
   arr: [1,2,3,4,5,6,7,8,9],


     }
   },

};
</script>

<template>

<ul>
	<template v-for="elem in arr">
		<li v-if="elem % 2 == 0">
			{{ elem }}
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


