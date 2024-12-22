<script>
export default {

	data() {
		return {
		arr: [],
		}
	},

	methods: {
	
	}
}
</script>

<template>
<p> Какой язык программирования вы выбираете  </p>
	<input type="checkbox" v-model="arr" value="JavaScrypt" id="checkbox">
	<label for="checkbox">JavaScrypt</label>
	<br>
	<input type="checkbox" v-model="arr" value="C++" id="checkbox">
	<label for="checkbox">C++</label>
	<br>
	<input type="checkbox" v-model="arr" value="Java" id="checkbox">
	<label for="checkbox">Java</label>
	<ul>
		<li v-for="item in arr">{{ item }}</li>
	</ul>
	

</template>


	<style scoped>

	</style>
