<script>
export default {

	data() {
		return {
			num1: '',
			num2: '',
			res: ''
		}
	},

	methods: {
		calc: function () {
			this.res = +this.num1 + +this.num2;
		}
	}
}
</script>

<template>
	<p>{{ res }}</p>
	<input v-model="num1">
	<input v-model="num2">
	<button @click="calc">work</button>
	</template>


	<style scoped>

	</style>
