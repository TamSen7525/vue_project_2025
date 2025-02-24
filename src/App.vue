<template>
  <div>
    <!-- Task 1 -->
    <h1>Task 1</h1>
    <button @click="showSum">Show Sum</button>

  </div>
</template>

<script>
export default {
  data() {
	return {
		num1: 1,
		num2: 2,
	}
  },
  methods: {
    showSum() {
      alert(this.num1 + this.num2);
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