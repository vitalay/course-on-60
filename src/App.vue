<script>
export default {

	data() {
		return {
		  message: ''
		}
	},

	methods: {

	}
}
</script>

<template>

<input type="number" v-model="message" placeholder="введите число">
<p>{{ message ** 2 }}</p>
</template>


<style scoped>

</style>
