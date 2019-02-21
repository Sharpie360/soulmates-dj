<template>
  <div class="about">
    <about--grid-container></about--grid-container>
    


    <div class="svg--bg-slice">
      <svg width="1447" height="703" viewBox="0 0 1447 703" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M1447 704.5C1047.8 28.0999 314.667 -37.6667 -2 14V704.5H1447Z" fill="url(#paint0_radial)"/>
        <defs>
        <radialGradient id="paint0_radial" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse" gradientTransform="translate(-1.99994 11.9999) rotate(25.1618) scale(1241.84 2555.02)">
        <stop stop-color="#330208"/>
        <stop offset="1" stop-color="#E81928"/>
        </radialGradient>
        </defs>
      </svg>
    </div>

  </div>
</template>

<script>
import About__GridContainer from '@/components/about_grid/About__GridContainer';

export default {
  components: {
    'about--grid-container': About__GridContainer,
  }
}
</script>

<style scoped>
.about {
  position: relative;
  height: calc(100% - 4rem);
}

.svg--bg-slice svg {
  position: absolute;
  bottom: 0;
  left: 0;
}
</style>
