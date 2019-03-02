<template>
  <div class="services--grid-container">
    <h1>Test</h1>
    <h1>Test</h1>
  </div>
</template>

<script>
import GridItem from '@/components/about_grid/GridItem';
export default {
  components: {
    
  }
}
</script>

<style scoped>
.services--grid-container {
  position: relative;
  z-index: 50;
  height: 100%;
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 1fr;


}
</style>
