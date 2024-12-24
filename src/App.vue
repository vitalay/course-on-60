<template>
	<User @show="func" />
</template>

<script>
import User from './components/User.vue';


export default {
	components: {
		User
	},
	data() {
		return {
			
		}
	},

	methods: {

		func(name, salary) {
			alert(name + '-' + salary + "$")
		},
	
		
	},

};
</script>

<style scoped>

</style>