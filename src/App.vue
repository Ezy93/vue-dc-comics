<template>
  <div id="app">
    <IndexHeader/>
    <Index-Main/>
  </div>
</template>

<script>
import IndexHeader from './components/IndexHeader.vue'
import IndexMain from './components/IndexMain.vue'

export default {
  name: 'App',
  components: {
    IndexHeader,
    IndexMain
  }
}
</script>

<style lang="scss">
@import "./assets/scss/style.scss";
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  
}
</style>
