
<script>
export default {
	data() {
		return {
			newItem: '', // Исправлено название переменной на camelCase
			items: ['a', 'b', 'c', 'd', 'e']
		};
	},
	methods: {
		removeItem(index) {
			this.items.splice(index, 1);
		},
		add() {
			if (this.newItem !== '') { // Проверка, чтобы избежать пустых значений
				this.items.unshift(this.newItem); // Добавляем новый элемент в начало массива
				this.newItem = ''; // Очищаем input поле
			}
		}
	}
};
</script>

<template>
	<input type="text" v-model="newItem">
	<button @click="add">Добавить</button>
	<ul>
		<li v-for="(item, index) in items" :key="index">
			{{ item }}
			<button @click="removeItem(index)">Удалить</button>
		</li>
	</ul>
</template>

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

