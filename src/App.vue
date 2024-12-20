
<template>
  <div>
    <a :href="href">{{ text }}</a>
   
  </div>
</template>

<script>
export default {
   data() {
     return {
      text: 'page',
      href: 'pages.html',
     }
   }
}
</script>



<style>

</style>


