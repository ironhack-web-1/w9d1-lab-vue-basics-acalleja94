<template>
  <div id="app">
    <NewHeader />

    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />

    <NewFooter />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import NewFooter from "./components/Footer.vue";
import NewHeader from "./components/Header.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    NewFooter,
    NewHeader
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
}
</style>
