<template>
  <div>
    <h1>Task 1</h1>
    <ul>
      <li v-for="(item, index) in items" :key="index" @click="removeItem(index)">
        {{ item }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: ["a", "b", "c", "d", "e"]
    };
  },
  methods: {
    removeItem(index) {
      this.items.splice(index, 1);
    }
  }
};
</script>