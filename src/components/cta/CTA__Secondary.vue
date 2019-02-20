<template>
  <router-link class="cta--outer cta--secondary flexbox-space-center pointer" tag="button" 
  :to="to">
    <span class="cta--inner">{{ text }}</span>
  </router-link>
</template>

<script>
export default {
  props: ['to', 'text']
}
</script>

<style scoped>
.cta--outer {
  position: relative;
  z-index: 50;
  padding: .5rem 2rem;
  border-radius: 50px;
}
.cta--inner {
  text-align: center;
  font-size: 200%;
  font-family: 'Advent Pro', sans-serif;
}
.cta--secondary {
  background-color: transparent;
  border: 2px solid var(--offBlack);
  color: var(--brightRed);
  font-weight: 500;
  transition: background-color .3s;
}
.cta--secondary:hover, .cta--secondary:active {
  background-color: rgb(253, 230, 230);
}
.cta--secondary:active {
  background-color: rgb(253, 230, 230);
  border: 2px solid var(--brightRed); 
}
</style>
