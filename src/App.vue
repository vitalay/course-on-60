<script>
export default {

	data() {
		return {
			selected: 'Тюмень',

		}
	},

	methods: {
	
	}
}
</script>

<template>
	<select v-model="selected">
		<option>Тюмень</option>
		<option>Москва</option>
		<option>Санкт-Петербург</option>
	</select>

	<p>{{ selected }}</p>

</template>


	<style scoped>

	</style>
