<template>
  <div id="app">
    <IndexHeader/>
    <Index-Main/>
    <IndexFooter/>
  </div>
</template>

<script>
import IndexHeader from './components/IndexHeader.vue'
import IndexMain from './components/IndexMain.vue'
import IndexFooter from './components/IndexFooter.vue'

export default {
  name: 'App',
  components: {
    IndexHeader,
    IndexMain,
    IndexFooter,
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
