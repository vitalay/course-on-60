<template>
  <div>
    <button @click="handle">btn</button>
 
  </div>
</template>

<script>
export default {
  emits: ['show'],
  data() {
    return {

    }
  },
  methods: {


    handle() {
      this.$emit('show' , 'Nick')
    },
 
  }

}
</script>