<template>
  <div>
    <!-- Task 1 -->
    <h1>Task 1</h1>
    <button @click="showDate">Show Date</button>

    <!-- Task 2 -->
    <h1>Task 2</h1>
    <button @mouseenter="showDate">Hover over me</button>
  </div>
</template>

<script>
export default {
  methods: {
    showDate() {
      alert(new Date());
    }
  }
};
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