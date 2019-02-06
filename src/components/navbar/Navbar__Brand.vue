<template>
  <div class="navbar-brand flex-1 flexbox flex-align-center">{{ brandText }}</div>
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

