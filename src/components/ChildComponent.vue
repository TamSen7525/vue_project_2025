<template>
    <div>
      <button @click="handleAction1">Call Function 1</button>
      <button @click="handleAction2">Call Function 2</button>
    </div>
  </template>
  
  <script>
  export default {
    emits: ['action1', 'action2'],
    methods: {
      handleAction1() {
        this.$emit('action1');
      },
      handleAction2() {
        this.$emit('action2');
      }
    }
  };
  </script>
  