<template>
  <div class="hero--container">

  <svg width="1920" height="800" viewBox="0 0 1920 800" fill="none" xmlns="http://www.w3.org/2000/svg">
    <path d="M0 603.826V0L1920 1.69297V603.826C1277.34 866.237 689.231 864.544 0 603.826Z" fill="#145656"/>
    <path d="M0 603.826V0L1920 1.69297V603.826C1277.34 866.237 689.231 864.544 0 603.826Z" fill="url(#paint0_linear)"/>
    <defs>
      <linearGradient id="paint0_linear" x1="960" y1="0" x2="960" y2="800" gradientUnits="userSpaceOnUse">
        <stop stop-color="#133D3D"/>
        <stop offset="1" stop-color="#146363"/>
      </linearGradient>
    </defs>
  </svg>


    <hero--brand-logo></hero--brand-logo>
    <div class="hero--text-group">
      <hero--header text="Soulmates git DJ"></hero--header>
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

<style>
.hero--container {
  position: absolute;
  width: 100%;
  z-index: 10;
  left: 0px;
  top: 0px;
}

.hero--text-group {
  position: relative;
  text-align: center;
  top: -15rem;
}

</style>
