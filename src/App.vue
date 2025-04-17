<template>
  <div>
    <h1>Task 1</h1>
    <select v-model="selectedDay">
      <option v-for="day in days" :key="day">{{ day }}</option>
    </select>
    <p>{{ selectedDay }}</p>

    <h1>Task 2</h1>
    <select v-model="selectedDate">
      <option v-for="date in dates" :key="date">{{ date }}</option>
    </select>
    <select v-model="selectedMonth">
      <option v-for="month in months" :key="month">{{ month }}</option>
    </select>
    <select v-model="selectedYear">
      <option v-for="year in years" :key="year">{{ year }}</option>
    </select>
    <p>{{ selectedDate }} {{ selectedMonth }} {{ selectedYear }}</p>

    <h1>Task 3</h1>
    <select v-model="currentDate">
      <option v-for="date in dates" :key="date">{{ date }}</option>
    </select>
    <select v-model="currentMonth">
      <option v-for="month in months" :key="month">{{ month }}</option>
    </select>
    <select v-model="currentYear">
      <option v-for="year in years" :key="year">{{ year }}</option>
    </select>
    <p>{{ currentDate }} {{ currentMonth }} {{ currentYear }}</p>
  </div>
</template>

<script>
export default {
  data() {
    const today = new Date();
    const months = [
      "January", "February", "March", "April", "May", "June",
      "July", "August", "September", "October", "November", "December"
    ];
    return {
      days: ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday"],
      selectedDay: "Monday",
      dates: Array.from({ length: 31 }, (_, i) => i + 1),
      months: months,
      years: Array.from({ length: 100 }, (_, i) => today.getFullYear() - i),
      selectedDate: 1,
      selectedMonth: "January",
      selectedYear: today.getFullYear(),
      currentDate: today.getDate(),
      currentMonth: months[today.getMonth()],
      currentYear: today.getFullYear()
    };
  }
};
</script>

<style>
body {
  font-family: Arial, sans-serif;
}
</style>