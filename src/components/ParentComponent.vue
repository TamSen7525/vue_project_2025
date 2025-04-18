<template>
    <div>
      <Employee 
        :name="'John'" 
        :salary="1000" 
        @sendName="func"
        @sendDetails="funcWithSalary" 
      />
    </div>
  </template>
  
  <script>
  import Employee from './components/Employee.vue'
  
  export default {
    methods: {
      func(name) {
        console.log(name);
      },
      funcWithSalary(name, salary) {
        console.log(name, salary);
      }
    },
    components: {
      Employee
    }
  };
  </script>
  