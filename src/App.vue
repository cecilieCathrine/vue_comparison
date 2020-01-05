<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <WhereToGo msg="Help! Where to go?"/>
  </div>
</template>

<script>
import WhereToGo from './components/WhereToGo.vue'

export default {
  name: 'app',
  components: {
    WhereToGo
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
