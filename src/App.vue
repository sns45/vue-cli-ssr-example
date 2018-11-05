<template>
  <div id="app">
    <HelloWorld parent="something" />
    <HelloWorld2 parent="something" />
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    HelloWorld : () => import('./components/HelloWorld.vue'),
    HelloWorld2 : () => import('./components/HelloWorld2.vue')
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
