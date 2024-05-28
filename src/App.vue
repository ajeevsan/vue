<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <!-- <TestComponnet message="Hello There"></TestComponnet> -->
    <DashboardComponent heading="Hello User" :options="['Home', 'Settings', 'Logout']" />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import TestComponnet from './components/TestComponnet.vue'
import DashboardComponent from './components/DashboardComponent.vue';

export default {
  name: 'App',
  components: {
    // TestComponnet,
    // HelloWorld
    DashboardComponent
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
}
</style>
