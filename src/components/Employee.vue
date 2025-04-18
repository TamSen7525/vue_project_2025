<template>
    <div>
      <button @click="sendName">Send Name</button>
      <button @click="sendDetails">Send Name and Salary</button>
    </div>
  </template>
  
  <script>
  export default {
    props: ['name', 'salary'],
    emits: ['sendName', 'sendDetails'],
    methods: {
      sendName() {
        this.$emit('sendName', this.name);
      },
      sendDetails() {
        this.$emit('sendDetails', this.name, this.salary);
      }
    }
  };
  </script>
  