<script>
export default {

	data() {
		return {
		checked: false
		}
	},

	methods: {
	
	}
}
</script>

<template>
	<input type="checkbox" v-model="checked">
<p v-if="checked" >{{ checked ? 'yes' : 'no' }}</p>
</template>


	<style scoped>

	</style>
