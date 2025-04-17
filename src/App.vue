<template>
  <div>
    <h1>Task 1</h1>
    <input v-model="newItem" />
    <button @click="addItem">Add</button>
    <ul>
      <li v-for="(item, index) in items" :key="index">{{ item }}</li>
    </ul>

    <h1>Task 2</h1>
    <input v-model="newItem2" />
    <button @click="addItemToStart">Add</button>
    <ul>
      <li v-for="(item, index) in items2" :key="index">{{ item }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      newItem: "",
      items: ["a", "b", "c", "d", "e"],
      newItem2: "",
      items2: ["a", "b", "c", "d", "e"]
    };
  },
  methods: {
    addItem() {
      if (this.newItem.trim()) {
        this.items.push(this.newItem);
        this.newItem = "";
      }
    },
    addItemToStart() {
      if (this.newItem2.trim()) {
        this.items2.unshift(this.newItem2);
        this.newItem2 = "";
      }
    }
  }
};
</script>