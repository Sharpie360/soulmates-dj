<template>
  <h1 class="hero--header">
    {{ text }}
  </h1>
</template>

<script>
export default {
  props: ['text'],
}
</script>

<style scoped>
.hero--header {
  font-family: 'Aclonica', sans-serif;
  font-weight: normal;
  font-size: 850%;
}
</style>

