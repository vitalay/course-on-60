<script>
export default {
   data() {
     return {
   
      //  dey: 0 // Здесь хранится номер дня недели
     };
   },
   methods: {
       show: function(nam) {
         alert('рузультат: ' + nam**2)
       }

    //  deys() {
    //    const result = this.dayOfTheWeek(this.dey); // Передаем значение dey в качестве аргумента
    //    return result;
    //  },
    //  dayOfTheWeek(num) {
    //    const days = [
    //      'Понедельник',
    //      'Вторник',
    //      'Среда',
    //      'Четверг',
    //      'Пятница',
    //      'Суббота',
    //      'Воскресенье'
    //    ];
    //    return days[num ]; // Возвращаем день недели по индексу
    //  }
   }
};
</script>

<template>
  <div>
    <!-- <h1 class="text-3xl font-bold underline">{{ cape(text) }}</h1>
    <p>{{ deys() }}</p> -->
    <button @click="show(2)">btn1</button>
    <button @click="show(3)">btn2</button>
  </div>
</template>


<style scoped>
.text-3xl{
  color: rgb(20, 151, 114)
}
</style>


