<template>
<table>
	<tr v-for="user in users" :key="user.id">
		
		<td>{{ user.name }}</td>
		<td>{{ user.salary }}</td>
		<td>{{ user.age }}</td>
		<td><a @click="removeItem(user.id)" href="#">delete</a></td>
	</tr>
</table>
</template>

<script>
export default {
	data() {
		return {
			users: [
				{
					id: 1,
					name: 'John',
					salary: '100',
					age: '20'
				},
				{
					id: 2,
					name: 'Bob',
					salary: '200',
					age: '30'
				},
				{
					id: 3,
					name: 'Alice',
					salary: '300',
					age: '40'
				}
			]
		};
	},

	methods: {
		// Метод для удаления элемента по ID
		removeItem(id) {
			this.users = this.users.filter(user => {
				return (user.id !== id);
			});
		}
	}
};
</script>

<style scoped>
table {
	border-collapse: collapse
}

td {
	border: 1px solid #ccc;
	padding: 10px;
}
</style>

