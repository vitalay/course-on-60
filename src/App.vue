<template>
	<E
		v-for="employee in employees"
		:key="employee.id"
		:name="employee.name"
		:salary="employee.salary"
		@remove="del"
	 />
</template>

<script>
import E from './components/E.vue';


export default {
	components: {
		E
	},
	data() {
		return {
			employees: [
				{
					id: 1,
					name: 'name1',
					salary: 10000
				},
				{
					id: 2,
					name: 'name2',
					salary: 5000
				},
				{
					id: 3,
					name: 'name3',
					salary: 7000
				},
			],	
	
		}
	},

	methods: {
		del(id) {
			this.employees = this.employees.filter((employee) => {
				return employee.id !== id;
			})
	
		}
	},

};
</script>

<style scoped>

</style>