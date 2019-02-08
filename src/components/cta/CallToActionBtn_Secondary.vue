<template>
  <router-link class="cta--outer cta--secondary flexbox-space-center" tag="div" 
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
  border-radius: 25px;
}
.cta--inner {
  text-align: center;
}
.cta--secondary {
  background-color: transparent;
  border: 2px solid var(--offBlack);
  color: var(--brightRed);
  font-weight: 600;
  transition: background-color .3s;
}
.cta--secondary:hover, .cta--secondary:active {
  background-color: rgb(253, 230, 230);
}
</style>
