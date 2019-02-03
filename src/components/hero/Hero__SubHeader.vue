<template>
  <h3 class="hero--sub-header">{{ text }}</h3>
</template>

<script>
export default {
  props: ['text']
}
</script>

<style scoped>
.hero--sub-header {
  font-weight: 300;
}
</style>
