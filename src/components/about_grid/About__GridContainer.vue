<template>
  <div class="about grid--container">
    <!-- grid item - title - use slots -->

    <grid--item :gridArea="pageTitle.gridArea">
      <h1 class="page-title flexbox flex-justify-end">
        {{ pageTitle.title }}
      </h1> 
    </grid--item>

    <grid--item :gridArea="mainText_ONE.gridArea">
      <div class="main-text--one--outer">
        <p class="main-text--one--inner">
          {{ mainText_ONE.text }}
        </p>
      </div>
    </grid--item>

  </div>
</template>

<script>
import GridItem from './GridItem';

export default {
  data () {
    return {
      pageTitle: {
        gridArea: '1 / 3 / span 1 / span 1',
        title: 'About',
      },
      mainText_ONE: {
        gridArea: '1 / 1 / span 1 / span 2',
        text: 'SoulmatesDJ is based in Minneapolis, MN - and has been providing great sounds and memories since 2015. With over 15 years of experince djing and hosting events of a wide variety, we know how to cater to the desires of you and your needs. We can handle as much or as little as you want us to. We are also happy to work along side other companies to make your visions a reality.'
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
  grid-template-columns: 3fr 10rem 1fr;
  grid-template-rows: 3fr 4fr 4fr;
}
.page-title {
  font-family: 'Aclonica';
  font-size: 500%;
  font-weight: 400;
  padding: 1rem 1.5rem;
}

.main-text--one--outer {
  margin: 1.5rem 2rem;
  padding: 1rem;
  background: linear-gradient(90deg, rgba(232, 25, 40, 0.2) 0%, rgba(255, 247, 247, 0) 100%);
  border-radius: 25px 0px 0px 25px;
}
.main-text--one--inner {
  font-size: 1.55rem;
  line-height: 1.6;
}

/* backdrop color */


</style>
