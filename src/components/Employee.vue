<!-- Employee.vue -->
<template>
    <div>
      <p>{{ name }} - {{ position }}</p>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        name: "John Doe",
        position: "Software Developer"
      };
    }
  };
  </script>
  