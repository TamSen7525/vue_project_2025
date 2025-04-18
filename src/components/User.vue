<template>
    <ul>
      <li v-for="(item, index) in arg" :key="index">{{ item }}</li>
    </ul>
  </template>
  
  <script>
  export default {
    props: ['arg']
  };
  </script>
  