<template>
  <div id="app">
    <IndexHeader/>
  </div>
</template>

<script>
import IndexHeader from './components/IndexHeader.vue'

export default {
  name: 'App',
  components: {
    IndexHeader
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
