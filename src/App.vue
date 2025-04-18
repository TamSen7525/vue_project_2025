<template>
  <div>
    <Employee :name="name" :salary="salary" :age="age" />
  </div>
</template>

<script>
import Employee from './components/Employee.vue'

export default {
  data() {
    return {
      name: 'John',
      salary: 50000,
      age: 30
    };
  },
  components: {
    Employee
  }
};
</script>