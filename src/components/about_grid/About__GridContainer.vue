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

    <grid--item :gridArea="mainText_TWO.gridArea">
      <div class="main-text--two--outer">
        <p class="main-text--two--inner">
          {{ mainText_TWO.text }}
        </p>
      </div>
    </grid--item>

    <grid--item :gridArea="mainText_THREE.gridArea">
      <div class="main-text--three--outer">
        <p class="main-text--three--inner">
          {{ mainText_THREE.text }}
        </p>
      </div>
    </grid--item>

    <subgrid gridArea=" 2 / 1 / span 3 / span 2 "></subgrid>

    <img
      style="grid-area: 1 / 3" 
      class="headphone-trace"
      src="../../assets/svg/headphones_trace_light-red.svg" alt="">

  </div>
</template>

<script>
import GridItem from './GridItem';
import Subgrid from './About__Subgrid';

export default {
  data () {
    return {
      pageTitle: {
        gridArea: '1 / 3 / span 1 / span 1',
        title: 'About',
      },
      mainText_ONE: {
        gridArea: '1 / 1 / span 2 / span 2',
        text: 'SoulmatesDJ is based in Minneapolis, MN - and has been providing great sounds and memories since 2015. With over 15 years of experince djing and hosting events of a wide variety, we know how to cater to the desires of you and your needs. We can handle as much or as little as you want us to. We are also happy to work along side other companies to make your visions a reality. SoulmatesDJ is based in Minneapolis, MN - and has been providing and memories since 2015.'
      },
      mainText_TWO: {
        gridArea: '2 / 2 / span 1 / span 2',
        text: 'Michelle Muse, a local veteran of the club and underground scene alike, she is best known for her sense of the utmost funk, and bridging the endless gaps of the genres of dance music. A mastress of her craft, Michelle is the right lady to keep the night vibes fine! A mastress of her craft, Michelle is the right lady to keep the night vibes fine!'
      },
      mainText_THREE: {
        gridArea: '4 / 3 / span 1 / span 1',
        text: 'Sean Crossphaize is the second half of the Soulmates duo, joining in the journey when along with his heart, his techincal skills complete Michelle’s personable likeness, making this duo a soulmates match for the ages. '
      },
      subGrid: {
        gridArea: '3 / 1 / span 2 / span 2'
      }
    }
  },
  components: {
    'grid--item': GridItem,
    'subgrid': Subgrid
  }
}
</script>

<style scoped>
.grid--container {
  height: 100%;
  display: grid;
  grid-template-columns: 3fr 10rem 1fr;
  grid-template-rows: 5fr 2rem 5fr 5fr;
}
.page-title {
  position: relative;
  z-index: 50;
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
}

.main-text--two--outer {
  margin: 0 1rem;
  padding: 1rem;
  background: linear-gradient(270deg, rgba(232, 25, 40, 0.2) 0%, rgba(255, 247, 247, 0) 60%);
  border-radius: 25px 25px 25px 25px;
}
.main-text--two--inner {
  font-size: 1.45rem;
  text-align: right;
}

.main-text--three--outer {
  margin: 0 1rem 1rem 1rem;
  padding: 1rem;
  background: linear-gradient(270deg, rgba(232, 25, 40, 0.2) 0%, rgba(255, 247, 247, 0) 80%);
  border-radius: 25px 25px 25px 25px;
}
.main-text--three--inner {
  font-size: 1.45rem;
  text-align: right;
}

.subgrid {
  position: relative;
  z-index: 50;
}

.headphone-trace {
  position: absolute;
  z-index: 0;
  top: 3rem;
  right: 3rem;
}

</style>
