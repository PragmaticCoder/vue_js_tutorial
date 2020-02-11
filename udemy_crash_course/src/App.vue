<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <TutorialComponent/>
  </div>
</template>

<script>
import TutorialComponent from "./components/TutorialComponent.vue"

export default {
  name: 'App',
  components: {
    TutorialComponent
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
