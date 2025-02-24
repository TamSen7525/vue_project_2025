<template>
  <div>
    <h1>Task 1</h1>
    <button @click="showCurrentDay">Show Current Day</button>
  </div>
</template>

<script>
export default {
  data() {
    return {}
  },
  methods: {
    showCurrentDay() {
      const today = new Date().getDay();
      const dayName = this.getDayName(today);
      alert(dayName);
    },
    getDayName(number) {
      const days = [
        'Воскресенье',
        'Понедельник',
        'Вторник',
        'Среда',
        'Четверг',
        'Пятница',
        'Суббота'
      ];
      return days[number] || 'Неверный номер дня';
    }
  }
}
</script>

<style scoped>
div {
  margin-bottom: 20px;
}

h1 {
  margin: 0 0 10px 0;
}

p {
  margin: 5px 0;
}
</style>