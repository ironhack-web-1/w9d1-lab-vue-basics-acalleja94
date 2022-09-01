<template>
    <Navbar msg="Welcome to Your Vue.js App"/>
  <img alt="Vue logo" src="./assets/logo.png">
  <Footer msg="Welcome to Your Vue.js App"/>

</template>

<script>
import navbar from './components/Navbar.vue'
import footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Footer
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
</style>
