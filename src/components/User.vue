<template>
  <div>
    <button @click="handle">btn</button>
    <button @click="handle1">btn1</button>
  </div>
</template>

<script>
export default {
  emits: ['show', 'show1'],
  data() {
    return {

    }
  },
  methods: {
/*************  ✨ Codeium Command ⭐  *************/
/**
 * Emits the 'show' event when the button is clicked.
 */

/******  93c34b5e-4464-49e7-857c-4c8c07227e76  *******/
    handle() {
      this.$emit('show')
    },
    handle1() {
      this.$emit('show1')
    }
  }

}
</script>