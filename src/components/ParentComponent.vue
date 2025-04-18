<template>
    <UserForm @add="add" />
  </template>
  
  <script>
  import UserForm from './UserForm.vue'
  
  export default {
    components: {
      UserForm
    },
    data() {
      return {
        users: []
      }
    },
    methods: {
      add(name, surn) {
        let id = this.users.length + 1;
        this.users.push({
          id,
          name,
          surn
        });
      }
    }
  }
  </script>
  