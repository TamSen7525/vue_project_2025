<template>
    <button @click="$emit('show')">
      Click Me
    </button>
  </template>
  
  <script>
  export default {
    emits: ['show'],
  };
  </script>
  