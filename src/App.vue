<template>
  <!-- Task 1 -->
  <div>
    <h1>Task 1</h1>
    <p>{{ arr[0] }}</p>
    <p>{{ arr[1] }}</p>
    <p>{{ arr[2] }}</p>
  </div>
  
  <!-- Task 2 -->
  <div>
    <h1>Task 2</h1>
    <p>{{ arr1[0] + arr1[1] + arr1[2] }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      arr: ['x', 'y', 'z'],
      arr1: [1, 2, 3],
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