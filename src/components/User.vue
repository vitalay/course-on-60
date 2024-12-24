<template>
 <br>
     {{ name }} 
     <br>
     {{ surn }}
     <br>
    <button @click="$emit('remove', id)">Удалить</button>
 <br>
</template>

<script>
export default {
  props: {
    id: Number,
    name: String,
    surn: String,
  },
  emits: ['remove'],
 
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