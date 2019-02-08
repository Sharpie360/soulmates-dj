<template>
  <div class="home">
    <hero--container></hero--container>
    <div class="cta--group pointer flexbox">
      <cta--primary 
        to="hire" 
        text="Hire Now!">
      </cta--primary>
      <div class="flex-spacer flex-1"></div>
      <cta--secondary 
        to="services" 
        text="Learn More">
      </cta--secondary>
    </div>

  </div>
</template>

<script>
// @ is an alias to /src
import Hero__Container from '@/components/hero/Hero__Container.vue';
import CallToActionBtn_Primary from '@/components/cta/CallToActionBtn_Primary';
import CallToActionBtn_Secondary from '@/components/cta/CallToActionBtn_Secondary';

export default {
  name: 'home',
  components: {
    'hero--container': Hero__Container,
    'cta--primary': CallToActionBtn_Primary,
    'cta--secondary': CallToActionBtn_Secondary,
  },
};
</script>

<style scoped>
.home {
  height: 100%;
}
.cta--group {
  position: relative;
  top: 42rem;
  width: 40%;
  margin: 0 auto;
}
</style>
