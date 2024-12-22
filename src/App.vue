<script>
export default {

	data() {
		return {
			text: '',
			arr: []
		}
	},

	methods: {
		split() {
			this.arr = this.text.split(' ')
		}
	}
}
</script>

<template>
<input v-model="text">
<button @click="split">click</button>
<ul>
	<li v-for="item in arr">{{ item }}</li>
</ul>
	</template>


	<style scoped>

	</style>
