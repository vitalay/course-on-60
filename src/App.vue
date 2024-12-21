<script>
export default {
   data() {
    return {
      dey: 'пт'
     }
   },
   methods: {

       
   },
   computed: {
    
   }

};
</script>

<template>
  <div>
<p v-if="dey === 'пн'">пн</p>
<p v-else-if="dey === 'вт'">вт</p>
<p v-else-if="dey === 'ср'">ср</p>
<p v-else-if="dey === 'чт'">чт</p>
<p v-else-if="dey === 'пт'">пт</p>
<p v-else-if="dey === 'сб'">сб</p>
<p v-else>вс</p>
  </div>
</template>


<style scoped>

</style>


