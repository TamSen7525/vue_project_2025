<template>
  <div>
    <h1>Task 1</h1>
    <button @click="showSquare(2)">Square of 2</button>
    <button @click="showSquare(3)">Square of 3</button>
  </div>
</template>

<script>
export default {
  data() {
    return {}
  },
  methods: {
    showSquare(number) {
      alert(number * number);
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