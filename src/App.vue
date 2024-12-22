<script>
export default {

	data() {
		return {
			text: '',

		}
	},

	methods: {
		toLeft() {
			this.text = 'Left'
		},

		toRight() {
			this.text = 'Right'
		},

		toMiddle() {
			this.text = 'Middle'
		}
	}
}
</script>

<template>

	<a 
	@click.prevent.left="toLeft"
  @click.prevent.right="toRight" 
	@click.prevent.middle="toMiddle"
	href="#"
	>Click
</a>
	{{ text }}

</template>


<style scoped></style>
<!-- 
Дана ссылка. Сделайте так, чтобы по нажатию левой кнопки мыши на эту ссылку в абзац под ссылкой вывелся текст 'left', по
нажатию правой кнопки мыши - текст 'right', а по нажатию средней кнопки - текст 'middle'. -->
