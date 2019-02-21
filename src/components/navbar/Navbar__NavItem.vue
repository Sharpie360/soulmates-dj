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
  text-decoration: none;
}
.navitem--outer:hover > .navitem--inner {
  border-bottom: 2px solid var(--offWhite);
}

.navitem--outer.router-link-exact-active {
  font-weight: 600;
}
.router-link-exact-active > .navitem--inner {
  font-weight: 500;
}

.navitem--inner {
  padding: .25rem .75rem;
  color: var(--offWhite);
  font-weight: 300;
  border-bottom: 2px solid transparent;
  border-bottom-left-radius: 15px;
  border-bottom-right-radius: 15px;
  transition: border .3s;
}

</style>
