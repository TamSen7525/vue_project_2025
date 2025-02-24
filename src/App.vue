<template>
  <div>
    <h1>Task 1</h1>
    <p>Cost: {{ cost }}</p>
    <p>Amount: {{ amount }}</p>
    <p>Total Price: {{ price }}</p>
    
    <h1>Task 2</h1>
    <button @click="changeCost">Change Cost</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      cost: 10,
      amount: 5
    }
  },
  computed: {
    price() {
      return this.cost * this.amount;
    }
  },
  methods: {
    changeCost() {
      this.cost = 20;
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