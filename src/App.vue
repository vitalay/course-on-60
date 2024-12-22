<script>
export default {
  name: 'App',
   data() {
    return {
			products: [
				{
					id:1,
					 name: 'product1',
				 },
				{
					id:2,
					 name: 'product2',
				 },
				{
					id:3,
					 name: 'product3',
				 },
			] 
     }
   },

};
</script>

<template>


	<template v-for="product in products" :key="product.id">
		<ul>
			{{ product.name }}
		</ul>
	
	</template>



</template>


<style scoped>
table {
  border: 1px solid black;
}
td {
	border: 1px solid black;
}
</style>


