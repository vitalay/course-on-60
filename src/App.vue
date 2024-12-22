<script>
export default {

	data() {
		return {
			text: '',
			result: ''
		}
	},

	methods: {
		toEnter() {
			this.result = this.text
		}
	}
}
</script>

<template>

<input @keyup.enter="toEnter" v-model="text">

{{ result }}

</template>


	<style scoped>

	</style>


<!-- Дан инпут. В этот инпут вводится текст. Сделайте так, чтобы по нажатию на клавишу Enter введенный текст появился в
абзаце под инпутом. -->
