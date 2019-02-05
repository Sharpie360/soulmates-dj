<template>
  <router-link class="flexbox flex-center" to="/">
    <span class="navitem--inner">{{ text }}</span>
  </router-link>
</template>

<script>
export default {
  props: ['text'],
}
</script>

<style>

</style>
