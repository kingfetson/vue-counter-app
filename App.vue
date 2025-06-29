<template>
  <main id="app">
    <h1 class="title">Hello, World!</h1>
    <button @click="incrementCounter">Increase</button>
    <button @click="decreaseCounter">Decrease</button>
    <p>Current Count: {{ counter }}</p>
  </main>
</template>

<script>
export default {
  data() {
    return {
      counter: 0,
    };
  },
  methods: {
    incrementCounter() {
      this.counter++;
    },
    decreaseCounter() {
      this.counter--;
    },
  },
};
</script>

<style>
#app {
  padding: 10px;
}

.title {
  color: blue;
}

button {
  margin-right: 10px;
  padding: 6px 12px;
  background-color: #eee;
  border: none;
  cursor: pointer;
  font-weight: bold;
  color: green;
}

p {
  margin-top: 15px;
  font-size: 18px;
}
</style>
