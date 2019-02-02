<template>
  <div class="home">
    <hero--container></hero--container>
  </div>
</template>

<script>
// @ is an alias to /src
import Hero__Container from '@/components/hero/Hero__Container.vue';

export default {
  name: 'home',
  components: {
    'hero--container': Hero__Container
  },
};
</script>
