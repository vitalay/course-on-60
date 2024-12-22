<script>
export default {

	data() {
		return {
			selectedDay: new Date().getDate(),
			days: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31],
			selectedMonth: new Date().getMonth() + 1,
			months: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
			selectedYear: new Date().getFullYear(),
			years: [2020, 2021, 2022, 2023, 2024],
		}
	},

	methods: {
	
	}
}
</script>

<template>
	<select v-model="selectedDay">
		<option v-for="day in days">{{ day }}</option>
	</select>
	<select v-model="selectedMonth">
		<option v-for="month in months">{{ month }}</option>
	</select>
	<select v-model="selectedYear">
		<option v-for="year in years">{{ year }}</option>
	</select>

	<p>{{ selectedDay }} {{ selectedMonth }} {{ selectedYear }}</p>

</template>


	<style scoped>

	</style>
