<template>
  <div id="app">
    <leftNav></leftNav>
    <router-view/>
  </div>
</template>

<script>
import leftNav from ./src/leftNav.vue
export default {
  name: 'app',
  components:{
    'leftNav':leftNav
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
