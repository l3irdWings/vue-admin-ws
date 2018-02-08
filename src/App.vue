<template>
  <div id="app">
    <div class="wrapper">
      <top-bar></top-bar>
      <router-view/>
    </div>
  </div>
</template>

<script>
import TopBar from './TopBar'

export default {
  name: 'app',
  components: {
    'top-bar': TopBar
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
