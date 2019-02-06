<template>
<div class="navbar--brand--outer flex-1 flexbox flex-align-center">
  <router-link to="/" tag="span" class="navbar-brand pointer">
    {{ brandText }}
  </router-link>
</div>
</template>

<script>
export default {
  props: ['brand-text']
}
</script>

<style scoped>
.navbar-brand {
  font-family: 'Aclonica', sans-serif;
  font-size: 1.25rem;
  margin-left: 1rem;
}
</style>

