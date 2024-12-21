<script>
export default {
  name: 'App',
   data() {
    return {
     
      products: [
			{
				name: 'product1',
				price: 100,
				quantity: 5
			},
			{
				name: 'product2',
				price: 200,
				quantity: 4
			},
			{
				name: 'product3',
				price: 300,
				quantity: 3
			},
		]


     }
   },

};
</script>

<template>


<table>
  <tr v-for="product in products">
    <td>{{ product.name }}</td>
    <td>{{ product.price }}</td>
    <td>{{ product.quantity }}</td>
  </tr>
</table>


<p v-for="num in 30">
		{{ num }}
	</p>

</template>


<style scoped>
table {
  border: 1px solid black;
}
td {
	border: 1px solid black;
}
</style>


