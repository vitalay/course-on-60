<script>
export default {

	data() {
		return {
		obj: {
				active: true,
				valid: false
		}
		}
	},

	methods: {

	}
}
</script>

<template>
	<p :class="{active: true, valid: false}">text</p>
</template>


<style scoped>

* {
	text-align: center;
}

</style>
