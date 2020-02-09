<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <News />
    <a href="https://newsapi.org/">Powered by News Api</a> 
  </div>
</template>

<script>
import News from './components/News.vue'

export default {
  name: 'app',
  components: {
    News
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
</style>
