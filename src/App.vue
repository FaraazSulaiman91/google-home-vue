<template>
  <div id="app">
    <GoogleHome/>
  </div>
</template>

<script>
import GoogleHome from './components/GoogleHome.vue'

export default {
  name: 'App',
  components: {
    GoogleHome
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
  height: 100%;
}
</style>
