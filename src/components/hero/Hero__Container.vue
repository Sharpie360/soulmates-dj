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
      <h1 class="hero--header">Soulmates DJ</h1>
      <h3 class="hero--sub-header">Give the best night of your life, the perfect soundtrack to match!</h3>
    </div>

  </div>
</template>

<script>

export default {
  props: ['']
  
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
.hero--header {
  font-family: 'Aclonica', sans-serif;
  font-weight: normal;
  font-size: 850%;
}
.hero--sub-header {
  font-weight: 300;
}
</style>
