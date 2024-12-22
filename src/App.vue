<script>
export default {

	data() {
		return {
		isDisabled: false,
		}
	},

	methods: {
	  //   toggleDisabled() {
		// 	this.isDisabled = !this.isDisabled;
		// }
	}
}
</script>

<template>
	<input type="text" :disabled="isDisabled">
  <!-- <button  @click="toggleDisabled">click</button> -->
	<input type="checkbox" v-model="isDisabled">

</template>


	<style scoped>

	</style>
