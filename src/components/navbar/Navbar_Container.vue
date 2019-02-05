<template>
  <div class="navbar--outer flexbox">
    <navbar--brand brandText="SoulmatesDJ"></navbar--brand>
    
    <router-link class="flexbox flex-center" to="/about">About</router-link>
  </div>
</template>

<script>
import Navbar_Brand from './Navbar_Brand';

export default {
  components: {
    'navbar--brand': Navbar_Brand,
  }
}
</script>

<style scoped>
.navbar--outer {
  position: relative;
  z-index: 50;
  height: 80px;
}

</style>
