<template>
  имя: {{ name }},
  <br>
  зарплата: {{ salary }},
  <br>
  года: {{ age }},
  
</template>

<script>
export default {
  props: ['name', 'salary', 'age'],
    data() {    
    
        return {
       
        
        }
    }
}
</script>

<style scoped>

</style>