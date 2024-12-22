<script>
export default {

	data() {
		return {
			text: '',
			arr: [],
		
		}
	},

	methods: {
		split() {
			this.arr = this.text.split(' ');
		}
	}
}
</script>

<template>
	<textarea v-model="text"></textarea>
	<button @click="split">Clear</button>
	<ul>
		<li v-for="word in arr">{{ word }}</li>
	</ul>
	
</template>


	<style scoped>

	</style>
