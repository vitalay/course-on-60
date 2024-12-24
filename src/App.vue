<template>
	<Employe :name="name" :salary="salary" :age="age" />



</template>

<script>
import Employe from './components/Employe.vue';
export default {
	components: {
		Employe
	},
	data() {
		return {
			name: 'Vladimir',
			salary: '100$',
			age: 22,
		
		}
	},

	methods: {
		
	},

};
</script>

<style scoped>

</style>