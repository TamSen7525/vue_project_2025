<template>
  <div>
    <h1>Task 1</h1>
    <input type="text" v-model="inputText" @keyup.enter="submitText" />
    <p>{{ displayedText }}</p>

    <h1>Task 2</h1>
    <a href="#" @click.ctrl.prevent="showCtrlMessage">Click me</a>
    <p>{{ ctrlMessage }}</p>

    <h1>Task 3</h1>
    <a href="#" @mousedown.left.prevent="setMouseText('left')" 
               @mousedown.right.prevent="setMouseText('right')" 
               @mousedown.middle.prevent="setMouseText('middle')">Click me</a>
    <p>{{ mouseText }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      inputText: "",
      displayedText: "",
      ctrlMessage: "",
      mouseText: ""
    };
  },
  methods: {
    submitText() {
      this.displayedText = this.inputText;
      this.inputText = "";
    },
    showCtrlMessage() {
      this.ctrlMessage = "Ctrl key was pressed!";
    },
    setMouseText(text) {
      this.mouseText = text;
    }
  }
};
</script>