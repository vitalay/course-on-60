<template>
 <br>
     {{ name }} 
     <br>
     {{ salary }}
     <br>
    <button @click="$emit('remove', id)">Удалить</button>
 <br>
</template>

<script>
export default {
  emits: ['remove'],
  props: {
    name: String,
    salary: Number,
    id: Number
  },
 
  data() {
    return {

    }
  },
  methods: {


    // handle() {
    //   this.$emit('show' , 'Nick', 500)
    // },
 
  }

}
</script>

<style scoped>

</style>