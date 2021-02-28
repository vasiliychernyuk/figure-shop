<template>
  <div id="app">
    <Header />
    <NavBar />
    <FirstLookSection />
  </div>
</template>

<script>
import Header from './components/main-header/main-header.vue';
import NavBar from './components/nav-bar/nav-bar.vue';
import FirstLookSection from './components/first-look-section/first-look-section.vue';

export default {
  name: 'App',
  components: {
    Header,
    NavBar,
    FirstLookSection
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Rubik:ital,wght@0,300;0,400;0,600;1,300;1,400;1,600&display=swap');
*{
  box-sizing: border-box;
  outline: none;
  border: none;
  list-style: none;
  text-decoration: none;
  margin: 0;
  padding: 0;
}
#app {
  font-family: 'Rubik', sans-serif;
  color: #333;
}
</style>
