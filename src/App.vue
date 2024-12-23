<template>
	<table>
		<tr v-for="user in users" :key="user.id">
			<!-- Обычный режим -->
			<td v-if="!user.isEdit">{{ user.name }}</td>
			<td v-else><input v-model="user.name" /></td>

			<td v-if="!user.isEdit">{{ user.salary }}</td>
			<td v-else><input v-model="user.salary" /></td>

			<td v-if="!user.isEdit">{{ user.age }}</td>
			<td v-else><input v-model="user.age" /></td>

			<!-- Кнопки редактирования и сохранения -->
			<td>
				<button v-if="!user.isEdit" @click="edit(user)">Редактировать</button>
				<button v-else @click="save(user)">Сохранить</button>
			</td>

			<!-- Кнопка удаления -->
			<td><button @click="removeItem(user.id)">Удалить</button></td>
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
					age: '20',
					isEdit: false
				},
				{
					id: 2,
					name: 'Bob',
					salary: '200',
					age: '30',
					isEdit: false
				},
				{
					id: 3,
					name: 'Alice',
					salary: '300',
					age: '40',
					isEdit: false
				}
			]
		};
	},

	methods: {
		// Метод для удаления элемента по ID
		removeItem(id) {
			this.users = this.users.filter(user => user.id !== id);
		},

		edit(user) {
			user.isEdit = true;
		},

		save(user) {
			user.isEdit = false;
		}
	}
};
</script>

<style scoped>
table {
	border-collapse: collapse;
}

td {
	border: 1px solid #ccc;
	padding: 10px 30px;
}

input {
	width: 70px;
}
</style>