<template>
  <HelloWorld msg="Simple Counter Application" />
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <p>Count: {{ count }}</p>
    <button v-on:click="increment">Increase Count</button>
    <button v-on:click="decrement">Decrease Count</button>
  </div>
</template>


<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  data() {
    return {
      count: 0
    };
  },
  components: {
    HelloWorld
  },
  methods: {
    increment: function () {
      this.count++;   // Increment the count
    },
    decrement: function () {
      this.count--;   // Decrement the count
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

p {
  font-size: 40px;
}

button {
  font-size: 20px;
  padding: 10px 20px 10px;
  ;
  border-radius: 5px;
  margin-left: 20px;
}
</style>
