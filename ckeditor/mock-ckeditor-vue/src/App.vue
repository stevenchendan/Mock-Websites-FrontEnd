<template>
  <div id="app">
    <NavigationBar></NavigationBar>
    <HomePage msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import HomePage from './components/HomePage.vue'
import NavigationBar from './components/NavigationBar'
export default {
  name: 'app',
  components: {
    HomePage,
    NavigationBar
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
html {
  font-size: 52.5%;
  font-family: 'Nunito Sans'
}
</style>
