<template>
  <div>
    <h1>Task 1</h1>
    <button @click="showDay">Show Day by Number</button>
    <h1>Task 2</h1>
    <button @click="showCurrentDay">Show Current Day</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      dayNumber: 3
    }
  },
  methods: {
    showDay() {
      const dayName = this.getDayName(this.dayNumber);
      alert(dayName);
    },
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