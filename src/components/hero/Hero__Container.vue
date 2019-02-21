<template>
  <div class="hero--container">

  <svg width="100%" viewBox="0 0 1920 850" fill="none" xmlns="http://www.w3.org/2000/svg">
  <path d="M0 641.566V0H1920V641.566C1277.34 920.377 689.231 918.578 0 641.566Z" fill="#E81928"/>
  <path d="M0 641.566V0H1920V641.566C1277.34 920.377 689.231 918.578 0 641.566Z" fill="url(#paint0_linear)"/>
  <defs>
    <linearGradient id="paint0_linear" x1="960" y1="0" x2="960" y2="850" gradientUnits="userSpaceOnUse">
      <stop stop-color="#E81928"/>
      <stop offset="1"/>
    </linearGradient>
  </defs>
</svg>
<hero--brand-logo></hero--brand-logo>
    <div class="hero--text-group">
      <hero--header text="Soulmates DJ"></hero--header>
      <hero--sub-header text="Give the best night of your life, the perfect soundtrack to match!"></hero--sub-header>
    </div>

  </div>
</template>

<script>
import Hero__BrandLogo from './Hero__BrandLogo';
import Hero__Header from './Hero__Header';
import Hero__SubHeader from './Hero__SubHeader';

export default {
  props: [''],
  components: {
    'hero--brand-logo': Hero__BrandLogo,
    'hero--header': Hero__Header,
    'hero--sub-header': Hero__SubHeader,
  }
}
</script>

<style scoped>
.hero--container {
  position: absolute;
  width: 100%;
  z-index: 10;
  left: 0px;
  top: 0px;
  color: var(--offWhite);
}

.hero--text-group {
  position: relative;
  text-align: center;
  top: -16rem;
}

</style>
