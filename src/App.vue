<script>
export default {

	data() {
		return {
			nevItem: '',
			items: ['a', 'b', 'c', 'd', 'e']
			
		}
	},

	methods: {
		add() {
			this.items.unshift(this.nevItem ) //добавление элемента в начало массива
			                                  //push - добавление элемента в конец массива
			                                  //shift -  удаление элемента в начале массива
		}
	}
}
</script>

<template>

<input type="text" placeholder="Введите текст" v-model="nevItem">
	<button @click="add">click</button>
	<ul>
		<li v-for="(item, index) in items" :key="index">
			{{ item }}
		</li>
	</ul>

</template>


<style scoped></style>


