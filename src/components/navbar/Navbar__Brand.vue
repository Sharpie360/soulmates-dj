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
  margin-left: 1rem;
}
</style>

