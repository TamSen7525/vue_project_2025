<template>
  <div>
    <p>{{ text }}</p>
    <button @click="change">Изменить текст</button>
    <button @click="changeToFirst">Первый текст</button>
    <button @click="changeToSecond">Второй текст</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      text: 'xxx'
    };
  },
  methods: {
    change() {
      this.text = 'yyy';
    },
    changeToFirst() {
      this.text = 'Первый';
    },
    changeToSecond() {
      this.text = 'Второй';
    }
  }
};
</script>

<style>
p {
  font-size: 18px;
  margin-bottom: 10px;
}
button {
  margin-right: 10px;
  padding: 5px 10px;
}
</style>