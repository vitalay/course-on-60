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
	<p v-for="item in arr">{{ item }}</p>

	</template>


	<style scoped>

	</style>
