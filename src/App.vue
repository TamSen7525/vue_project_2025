<template>
  <div>
    <Employee name="John" surn="Doe" age="30" />
  </div>
</template>

<script>
import Employee from './components/Employee.vue'

export default {
  components: {
    Employee
  }
};
</script>