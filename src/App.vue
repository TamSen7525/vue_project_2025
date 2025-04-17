<template>
  <div>
    <h1>Task 1</h1>
    <input type="text" :disabled="isDisabled" />
    <button @click="toggleInput">{{ isDisabled ? "Unlock" : "Lock" }}</button>

    <h1>Task 2</h1>
    <input type="checkbox" v-model="isChecked" />
    <input type="text" :disabled="!isChecked" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      isDisabled: true,
      isChecked: false
    };
  },
  methods: {
    toggleInput() {
      this.isDisabled = !this.isDisabled;
    }
  }
};
</script>