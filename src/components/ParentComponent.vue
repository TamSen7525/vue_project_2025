
<template>
    <div>
      <Employee @show="handleClick" />
    </div>
  </template>
  
  <script>
  import Employee from './components/Employee.vue';
  
  export default {
    methods: {
      handleClick() {
        console.log('Button was clicked!');
      }
    },
    components: {
      Employee
    }
  };
  </script>
  
