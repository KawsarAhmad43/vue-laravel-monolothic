<template>
    <div>
      <h1>Hello from Vue.js!</h1>
      <button @click="showMessage">Click me</button>
      <p v-if="message">{{ message }}</p>
    </div>
  </template>

  <script>
  export default {
    name: 'App',
    data() {
      return {
        message: ''
      };
    },
    methods: {
      showMessage() {
        this.message = 'Hello from Vue!';
      }
    }
  };
  </script>

  <style scoped>
  /* Scoped styles for this component */
  </style>
