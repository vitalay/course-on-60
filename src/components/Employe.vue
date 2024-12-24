<template>
  <table>
    <tr>
      <td>{{ name }}</td>
      <td>{{ age }}</td>
      <td>{{ salary }}</td>
    </tr>
  </table>



</template>

<script>
export default {
  props: {
    key: Number,
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
table {
  border-collapse: collapse;
  width: 100%;
}

td, th {
  border: 1px solid #ddd;
  padding: 8px;
}

tr:nth-child(even){background-color: #f2f2f2;}

</style>