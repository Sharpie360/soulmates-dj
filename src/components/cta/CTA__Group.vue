<template>
  <div class="cta--group flexbox">
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
</template>

<script>
import CTA__Primary from './CTA__Primary';
import CTA_Secondary from './CTA__Secondary';

export default {
  components: {
    'cta--primary': CTA__Primary,
    'cta--secondary': CTA_Secondary
  }
}
</script>

<style scoped>
.cta--group {
  position: relative;
  top: 42rem;
  width: 40%;
  margin: 0 auto;
}
</style>
