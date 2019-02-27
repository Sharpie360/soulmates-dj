<template>
  <div class="services-view--outer">

    <services--grid></services--grid>

    <div class="svg--bg-swoop">
      <svg width="1476" height="1000" viewBox="0 0 1476 1000" fill="none" xmlns="http://www.w3.org/2000/svg">
      <path d="M599.44 520.26C581.178 128.864 194.487 0.263196 0 0H1476V1001H1238.6C1033.61 1001 617.701 911.655 599.44 520.26Z" fill="url(#paint0_linear)"/>
      <defs>
        <linearGradient id="paint0_linear" x1="338.754" y1="34.5173" x2="1507.98" y2="506.581" gradientUnits="userSpaceOnUse">
          <stop stop-color="#14021D"/>
          <stop offset="1" stop-color="#E81928"/>
        </linearGradient>
      </defs>
    </svg>

    </div>
  </div>
</template>

<script>
import Services_GridContainer from '../components/services/_grid/Services_GridContainer';

export default {
  components: {
    'services--grid': Services_GridContainer,
  }
}
</script>

<style scoped>
.services-view--outer {
  height: calc(100% - 4rem);
  overflow-x: hidden !important;
}
.svg--bg-swoop svg {
  position: absolute;
  top: 4rem;
  right: 0;
  z-index: 0;
}

</style>

