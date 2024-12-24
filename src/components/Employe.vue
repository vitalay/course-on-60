<template>
  имя: {{ name }},
  <br>
  зарплата: {{ salary }},
  <br>
  года: {{ age }},
  
</template>

<script>
export default {
  props: {
    name: String,
    salary: Number,
    age: Number
  },
    data() {    
    
        return {
       
        
        }
    }
}
</script>

<style scoped>

</style>