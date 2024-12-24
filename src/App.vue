<template>
	<User @show="func" @show1="func1"/>
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
		func() {
			alert('123')
		},
		func1() {
			alert('222')
		}
		
	},

};
</script>

<style scoped>

</style>