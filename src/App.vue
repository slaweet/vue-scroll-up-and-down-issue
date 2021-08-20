<template>
  <div id="app">
    <p v-for="i in 100" :key="i" class="alert alert-info m-3" > Mock element no. {{i}}</p>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <scroll-up />
  </div>
</template>

<script>
import 'vue-scroll-up/dist/style.css'
import ScrollUp from 'vue-scroll-up'
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    ScrollUp
  }
}
</script>

<style lang="css" src="bootstrap/dist/css/bootstrap.css"></style>
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
