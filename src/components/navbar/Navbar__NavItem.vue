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
  color: var(--fontColorHeadings);
  text-decoration: none;
}
.navitem--outer:hover > .navitem--inner {
  border-bottom: 2px solid var(--fontColorHeadings);
}

.navitem--outer.router-link-exact-active {
  color: var(--fontColorHeadings);
  font-weight: 600;
}
.router-link-exact-active > .navitem--inner {
  font-weight: 500;
}

.navitem--inner {
  padding: .5rem .25rem;
  color: var(--fontColorHeadings);
  font-weight: 300;
  border-bottom: 2px solid transparent;
  transition: border .3s;
}

</style>
