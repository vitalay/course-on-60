<template>
	<User 
	v-for="user in users"
	 :id="user.id"
	  :name="user.name" 
		:surn="user.surn" 
		:key="user.id"
		 @change="change"
		  />
	<EmploeForme 
	@add="add"
	
	/>
</template>

<script>
import User from './components/User.vue';
import EmploeForme from './components/EmploeForme.vue';

export default {
	components: {
		User,
		EmploeForme
	},
	data() {
		return {
			users: [
				{
					id: 1,
					name: 'name1',
					surn: 'surn1'
				},
				{
					id: 2,
					name: 'name2',
					surn: 'surn2'
				},
				{
					id: 3,
					name: 'name3',
					surn: 'surn3'
				},
			],
	
		}
	},

	methods: {
		
		change(id, name, surn) {
			this.users = this.users.map((user) => {
				if (user.id === id) {
					user.name = name;
					user.surn = surn;
				}
				return user;
			});
		},
		add(name, surn) {
			this.users.push({
				id: this.users.length + 1,
				name,
				surn
			});
		}
	},

};
</script>

<style scoped>

</style>