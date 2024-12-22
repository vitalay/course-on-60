<script>
export default {

	data() {
		return {
			isActive: false,
			hasError: true,
		}
	},

	methods: {

	}
}
</script>

<template>
	<p :class="{ active: isActive, error: hasError }">
		text
	</p>
</template>


<style scoped>
* {
	text-align: center;
}
</style>
