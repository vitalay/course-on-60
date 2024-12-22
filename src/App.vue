<script>
export default {

	data() {
		return {
		obj: {
				hidden: true,
		}
		}
	},
	methods: {
		show () {
			this.obj.hidden = !this.obj.hidden
		}
	}
};
</script>

<template>
	<p :class="obj">text</p>
	<button @click="show">done</button>

</template>


<style scoped>

p.hidden {
	display: none;
}

</style>
