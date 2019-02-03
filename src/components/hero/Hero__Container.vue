<template>
  <div class="hero--container">
    <svg width="100%" viewBox="0 0 1920 750" fill="none" xmlns="http://www.w3.org/2000/svg">
      <path d="M0 566.087V0L1920 1.58716V566.087C1277.34 812.097 689.231 810.51 0 566.087Z" fill="#145656"/>
      <path d="M0 566.087V0L1920 1.58716V566.087C1277.34 812.097 689.231 810.51 0 566.087Z" fill="url(#paint0_linear)"/>
      <defs>
      <linearGradient id="paint0_linear" x1="960" y1="0" x2="960" y2="750" gradientUnits="userSpaceOnUse">
      <stop stop-color="#133D3D"/>
      <stop offset="1" stop-color="#146363"/>
      </linearGradient>
      </defs>
    </svg>
    
    <div class="hero--text-group">
      <hero--header text="Soulmates DJ"></hero--header>
      <hero--sub-header text="Give the best night of your life, the perfect soundtrack to match!"></hero--sub-header>
    </div>

  </div>
</template>

<script>
import Hero__Header from './Hero__Header';
import Hero__SubHeader from './Hero__SubHeader';

export default {
  props: [''],
  components: {
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
  top: -18rem;
}

</style>
