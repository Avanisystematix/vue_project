<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Home data="hey"/>
    <ComposingWithComponent/>
    <TemplateWithExample/>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import Home from './components/Home.vue'
// import ComposingWithComponent from './components/ComposingWithComponent.vue'
import TemplateWithExample from './components/TemplateWithExample.vue';

export default {
  name: 'App',
  components: {
    // HelloWorld,
    // Home,
    // ComposingWithComponent,
    TemplateWithExample
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
