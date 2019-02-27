<template>
  <router-link 
    class="
      cta--outer 
      cta--primary 
      flexbox-space-center 
      pointer" 
    tag="button" 
    to="/">

    <span 
      class="cta--inner"
      >{{ text }}
    </span>

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
  padding: .75rem 4rem;
  border-radius: 50px;
}
.cta--inner {
  text-align: center;
  font-size: 1.8rem;
  font-family: 'Anaheim';
}
.cta--primary {
  color: var(--offWhite);
  background-color: var(--brightRed);
  border: 2px solid var(--offBlack);
  font-weight: 400;
  transition: background-color .3s;
}
.cta--primary:hover, .cta--primary:active {
  background-color: var(--brightestRed);
}
</style>
