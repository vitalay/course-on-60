
<template>
  <!-- Контейнер для основной информации -->
  <div class="template-container" v-if="!isEdit">
    <!-- Отображаем имя и фамилию -->
    <span class="name">{{ name }}</span>
    <span class="surname">{{ surn }}</span>

    <!-- Кнопка редактирования -->
    <button @click="edit">Редактировать</button>
  </div>

  <!-- Контейнер для формы редактирования -->
  <div class="template-container" v-else>
    <!-- Поле ввода нового имени -->
    <input type="text" v-model="newName" placeholder="Имя" />

    <!-- Поле ввода новой фамилии -->
    <input type="text" v-model="newSurn" placeholder="Фамилия" />

    <!-- Кнопка сохранения изменений -->
    <button @click="save">Сохранить</button>
  </div>
</template>

<script>
export default {
  props: {
    id: Number,
    name: String,
    surn: String,
  },
  emits: ["change"],
  data() {
    return {
      isEdit: false,
      newName: this.name,
      newSurn: this.surn,
    };
  },
  methods: {
    // Метод для перехода в режим редактирования
    edit() {
      this.isEdit = true;
    },
    // Метод для сохранения изменений
    save() {
      this.isEdit = false;
      this.$emit("change", this.id, this.newName, this.newSurn);
    },
  },
};
</script>

<!-- Локальные стили для этого компонента -->
<style scoped>
/* Основные стили контейнера */
.template-container {
  border: 1px solid #ccc;
  padding: 10px;
  margin-bottom: 20px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

/* Стилизация имени и фамилии */
.name,
.surname {
  font-size: 16px;
  color: #333;
  margin-right: 10px;
}

/* Стилизация кнопок */
button {
  background-color: #4caf50;
  color: white;
  padding: 8px 12px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  cursor: pointer;
  border-radius: 4px;
  border: none;
  outline: none;
}

button:hover {
  background-color: #45a049;
}

/* Стилизация полей ввода */
input {
  padding: 6px 10px;
  border: 1px solid #ccc;
  border-radius: 4px;
  width: 150px;
  margin-right: 10px;
}
</style>