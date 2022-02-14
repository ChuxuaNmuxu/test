<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <SlotComp>
      <HelloWorld msg="Welcome to Your Vue.js App"/>
    </SlotComp>
  </div>
</template>

<script>
import SlotComp from './components/slotComp.vue'

export default {
  name: 'App',
  components: {
    SlotComp,
    HelloWorld: () => import('./components/HelloWorld.vue')
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
