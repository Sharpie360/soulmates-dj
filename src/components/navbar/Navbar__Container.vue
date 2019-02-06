<template>
  <div class="navbar--outer flexbox">
    <navbar--brand brand-text="SoulmatesDJ"></navbar--brand>
    <navbar--navitem to="/" text="Home"></navbar--navitem>
    <navbar--navitem to="about" text="About"></navbar--navitem>
    <navbar--navitem to="services" text="Services"></navbar--navitem>
    <navbar--navitem to="hire" text="Hire"></navbar--navitem>
  </div>
</template>

<script>
import Navbar__Brand from './Navbar__Brand';
import Navbar__NavItem from './Navbar__NavItem';

export default {
  components: {
    'navbar--brand': Navbar__Brand,
    'navbar--navitem': Navbar__NavItem
  }
}
</script>

<style scoped>
.navbar--outer {
  position: relative;
  z-index: 50;
  height: 4rem;
}

</style>
