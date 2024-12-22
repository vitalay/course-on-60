<script>
export default {

	data() {
		return {
			arr: ['a', 'b', 'v', 'q', 'c'],

		}
	},
	methods: {
		add() {
			this.arr.pop()

		},
		add2() {
			this.arr.push('d')
		},
		del() {
			this.arr.splice(-2, 1)
		},
		del2() {
			this.arr.sort()
		},
		add3() {
			this.arr.reverse()
		}

	}

};
</script>

<template>
	<ul>
		<li v-for="elem in arr">
			{{ elem }}
		</li>
	</ul>

	<button @click="add">Удалить</button>
	<button @click="add2">Добавить</button>
	<button @click="del">Удалить предпоследний</button>
	<button @click="del2">Сортировать</button>
	<button @click="add3">Перевернуть</button>



</template>


<style scoped>
table {
	border: 1px solid black;
}

td {
	border: 1px solid black;
}
</style>
