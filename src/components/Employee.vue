<template>
    <div>
      <p>Name: {{ name }}</p>
      <p>Surname: {{ surn }}</p>
      <p>Age: {{ age }}</p>
    </div>
  </template>
  
  <script>
  export default {
    props: ['name', 'surn', 'age']
  };
  </script>
  