<template>
  <div class="about grid--container">
    <!-- grid item - title - use slots -->
    <grid--item :gridArea="pageTitle.gridArea">
      <h1 class="page-title flexbox flex-justify-end">
        {{ pageTitle.title }}
      </h1> 
      <h2 
        slot="secondary" class="flexbox-space-center">our company!</h2>
    </grid--item>
  </div>
</template>

<script>
import GridItem from './GridItem';

export default {
  data () {
    return {
      pageTitle: {
        gridArea: '1 / 2 / span 1 / span 1',
        title: 'About',
      }
    }
  },
  components: {
    'grid--item': GridItem,
  }
}
</script>

<style scoped>
.grid--container {
  height: 100%;
  display: grid;
  grid-template-columns: 2fr 1fr;
  grid-template-rows: 3fr 4fr 4fr;
}
.page-title {
  font-family: 'Aclonica';
  font-size: 500%;
  font-weight: 400;
  padding: 1rem 1.5rem;
}
</style>
