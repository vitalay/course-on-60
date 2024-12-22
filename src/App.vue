<script>
export default {

	data() {
		return {
			choice: '',

		}
	},

	methods: {
	
	}
}
</script>

<template>
	<p> Какой язык для вас родной</p>
	<input name="radio" type="radio" v-model="choice" value="на улице идет дождь">
	<label for="Русский">Русский</label>
	<br>
	<input name="radio" type="radio" v-model="choice" value="it's raining outside
">
	<label for="Английский">Английский</label>
	<br>
	<input name="radio" type="radio" v-model="choice" value="Draußen regnet es
">
	<label for="Неметский">Неметский</label>

	<p v-if="choice" >{{ choice }}</p>
	<p v-else>на улице идет дождь</p>
	<p></p>

</template>


	<style scoped>

	</style>
