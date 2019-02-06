<template>
  <router-link class="navitem--outer flexbox flex-center" :to="to">
    <span class="navitem--inner">{{ text }}</span>
  </router-link>
</template>

<script>
export default {
  props: ['to','text'],
}
</script>

<style>

.navitem--outer {
  width: 8rem;
  color: #f7f7f7;
}

.navitem--outer.router-link-exact-active {
  color: #42b983;
}
</style>
