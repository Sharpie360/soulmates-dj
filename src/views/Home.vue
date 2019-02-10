<template>
  <div class="home">
    <hero--container></hero--container>
    <cta--group></cta--group>
  </div>
</template>

<script>
// @ is an alias to /src
import Hero__Container from '@/components/hero/Hero__Container.vue';
import CTA__Group from '@/components/cta/CTA__Group';

export default {
  name: 'home',
  components: {
    'hero--container': Hero__Container,
    'cta--group': CTA__Group
  },
};
</script>

<style scoped>
.home {
  height: 100%;
}

</style>
