<template>
  <div id="app">
    <div id="nav" class="flexbox">
      <div class="navbar-brand flex-1 flexbox flex-align-center">Soulmates DJ</div>
      <router-link class="flexbox flex-center" to="/">
        <div class="navitem--inner">Home</div>
      </router-link>
      <router-link class="flexbox flex-center" to="/about">About</router-link>
    </div>
    <router-view :clientWidth="clientWidth" :clientHeight="clientHeight"/>
  </div>
</template>

<script>


export default {
  data () {
    return {
      clientWidth: 0,
      clientHeight: 0,
    }
  },
  mounted() {
    this.$nextTick(() => {
      window.addEventListener('resize', this.getClientWidth);
      window.addEventListener('resize', this.getClientHeight);
      this.getClientWidth();
      this.getClientHeight();
    })
  },
  methods: {
    getClientWidth () {
      this.clientWidth = document.documentElement.clientWidth;
    },
    getClientHeight () {
      this.clientHeight = document.documentElement.clientHeight;
    }
  },
  beforeDestroy() {
    window.removeEventListener('resize', this.getClientWidth);
    window.removeEventListener('resize', this.getClientHeight);
  },
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
#nav {
  position: relative;
  z-index: 50;
  height: 80px;
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
