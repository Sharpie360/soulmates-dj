<template>
  <div id="app">
    <app--navbar></app--navbar>
    <router-view />
  </div>
</template>

<script>
import Navbar_Container from './components/navbar/Navbar_Container';

export default {
  components: {
    'app--navbar': Navbar_Container,
  }
}
</script>

<style>

@import './assets/css/main.css';
@import './assets/css/flexbox-util.css';
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #f7f7f7;
  background-color: var(--backgroundMain);
  height: 100%;
}

.navbar-brand {
  margin-left: 1rem;
}

#nav a {
  width: 8rem;
  color: #f7f7f7;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
