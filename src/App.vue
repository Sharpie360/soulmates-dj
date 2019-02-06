<template>
  <div id="app">
    <app--navbar></app--navbar>
    <router-view />
  </div>
</template>

<script>
import Navbar__Container from './components/navbar/Navbar__Container';

export default {
  components: {
    'app--navbar': Navbar__Container,
  }
}
</script>

<style>

@import './assets/css/main.css';
@import './assets/css/flexbox-util.css';
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  height: 100%;
}

</style>
