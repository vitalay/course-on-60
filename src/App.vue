<script>
export default {

	data() {
		return {
			text: '',
			
		}
	},

	methods: {
		toShift() {
			this.text = 'Hello'
		}
	}
}
</script>

<template>

	<a @click.prevent.shift.exact="toShift" href="#">Click</a>
	{{ text }}

</template>


	<style scoped>

	</style>

<!-- Дана ссылка. Сделайте так, чтобы по клику на эту ссылку, если в этот момент зажата клавиша Ctrl, в абзац под ссылкой
вывелся какой-нибудь текст.
 -->
