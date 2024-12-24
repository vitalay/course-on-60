<template>
  <div>
    <button @click="$emit('show', 'Nick', 500)">btn</button>
 
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


    // handle() {
    //   this.$emit('show' , 'Nick', 500)
    // },
 
  }

}
</script>