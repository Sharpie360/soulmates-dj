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

<style scoped>
.navitem--outer {
  width: 7rem;
  color: #f7f7f7;
  text-decoration: none;
}
.navitem--outer:hover > .navitem--inner {
  border-bottom: 2px solid var(--fontColorMain);
}

.navitem--outer.router-link-exact-active {
  color: #ffffff;
}

.navitem--inner {
  padding: .5rem .25rem;
  color: #ffffff;
  font-weight: 300;
  border-bottom: 2px solid transparent;
}

</style>
