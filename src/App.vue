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
/*************  ✨ Codeium Command ⭐  *************/
		/**
		 * Shows alert box with given name
		 * @param {string} name
		 */
/******  111cd865-5977-4bd7-bf9d-96d6e0561b30  *******/
		func(name) {
			alert(name)
		},
	
		
	},

};
</script>

<style scoped>

</style>