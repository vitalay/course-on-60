<script>
export default {

	data() {
		return {
			num1: '',
			num2: '',
			temp: ''
		}
	},

	methods: {
		change: function () {
			this.temp = this.num1;
			this.num1 = this.num2;
			this.num2 = this.temp;
		}
	}
}
</script>

<template>
	<p>{{ temp }}</p>
	<input v-model="num1">
	<input v-model="num2">
	<button @click="change">work</button>
	</template>


	<style scoped>

	</style>
