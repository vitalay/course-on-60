<template>
	<div>
		<!-- Список пользователей -->
		<ul>
			<li v-for="user in users" :key="user.id">
				Зарплата: {{ user.salary }} Лет {{ user.age }} Имя {{ user.name }}
				<!-- Кнопка удаления для каждого элемента -->
				<button @click="removeItem(user.id)">Удалить</button>
			</li>
		</ul>
	</div>
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
			this.users = this.users.filter(user => user.id !== id);
		}
	}
};
</script>

<style scoped>
/* Основные стили */
body {
	font-family: Arial, sans-serif;
	background-color: #f4f4f4;
	margin: 0;
	padding: 20px;
}

ul {
	list-style-type: none;
	padding: 0;
	margin-bottom: 10px;
}

li {
	display: flex;
	align-items: center;
	justify-content: space-between;
	border: 1px solid #ccc;
	padding: 10px;
	margin-bottom: 5px;
	background-color: white;
	border-radius: 5px;
}

button {
	cursor: pointer;
	padding: 8px 12px;
	border: none;
	color: white;
	background-color: #007BFF;
	border-radius: 5px;
	transition: background-color 0.3s ease;
}

button:hover {
	background-color: #0056b3;
}

input[type=text] {
	width: 100%;
	padding: 10px;
	margin-right: 10px;
	border: 1px solid #ccc;
	border-radius: 5px;
}

/* Дополнительный стиль для кнопки удаления */
.remove-button {
	background-color: #dc3545;
}

.remove-button:hover {
	background-color: #b02a37;
}
</style>

