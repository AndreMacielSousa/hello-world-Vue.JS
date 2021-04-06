<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <Dog breed="bulldog" />
  </div>
</template>

<script>

import HelloWorld from "./components/HelloWorld.vue";

import Dog from "./components/Dog.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    Dog,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  background-color: rgba(238, 255, 0, 0.274);
}
</style>
