<template>
  <div id="app">
    <Header />
  </div>
</template>

<script>
import Header from './components/main-header/main-header.vue';
export default {
  name: 'App',
  components: {
    Header,
  }
}
</script>

<style>
body{ margin: 0; }
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
