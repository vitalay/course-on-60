<template>
  <ul>
    <li v-for="arg in items">{{ arg }}</li>
    
  </ul>
</template>

<script>
export default {
  props: ['arg'],
    data() {    
    
        return {
          items: this.arg

        
        }
    }
}
</script>

<style scoped>

</style>