<template>
  <div>
     <input type="text" v-model="newName" placeholder="Имя">
     <input type="text" v-model="newSurn" placeholder="Фамилия">
     <button @click="save">save</button>
  </div>
</template>

<script>
export default {
  emits: ['add'],
  props: {
    id: Number,
    nane: String,
    surn: String
  },
  data() {
    return {
      newName: '',
      newSurn: '',
    }
  },
  methods: {
    save() {
      this.$emit('add', this.newName, this.newSurn)
    }
  }
}

</script>

<style scoped>

</style>