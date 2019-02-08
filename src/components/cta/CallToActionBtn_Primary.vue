<template>
  <router-link class="cta--outer cta--primary flexbox-space-center" tag="div" 
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
.cta--primary {
  color: var(--fontColorHeadings);
  background-color: var(--brightRed);
  border: 2px solid var(--offBlack);
  font-weight: 400;
  transition: background-color .3s;
}
.cta--primary:hover, .cta--primary:active {
  background-color: var(--brightRed-dark);
}
</style>
