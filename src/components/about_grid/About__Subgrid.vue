<template>
  <div
    :style="{ 'grid-area': gridArea }" 
    class="about--subgrid">

    <grid--item :gridArea="focusArea.title.gridArea">
      <div class="
        focus-area--title--outer
        flexbox flex-1 flex-align-flexend
        ">
        <h2 class="focus-area--title--inner">
          {{ focusArea.title.text }}
        </h2>
      </div>
    </grid--item>

    <grid--item :gridArea="focusArea.text_ONE.gridArea">
      <div class="focus-area--text-one--outer flexbox-space-center">
        <p class="focus-area--text-one--inner">
          {{ focusArea.text_ONE.text }}
        </p>
      </div>
    </grid--item>

    <grid--item :gridArea="focusArea.text_TWO.gridArea">
      <div class="focus-area--text-two--outer">
        <p class="focus-area--text-two--inner">
          {{ focusArea.text_TWO.text }}
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
      focusArea: {
        title: {
          gridArea: ' 1 / 1 / span 1 / span 2 ',
          text: 'What We Do'
        },
        text_ONE: {
          gridArea: ' 2 / 1 / span 1 / span 2 ',
          text: 'We keep the night groovin! Specializing in crushin\' up the decks, our club-hardened DJ\'s know exactly how to keep the dance floor full and moving!',
        },
        text_TWO: {
          gridArea: ' 3 / 1 / span 1 / span 3 ',
          text: 'With an expansive blend of top tracks and underground sounds, you can be sure that soulmatesDJ isn’t your typical "Press Play" DJ company. With our DJ’s, your guests won’t be able to resist the dance!'
        }
      }
    }
  },
  props: ['gridArea'],
  components: {
    'grid--item': GridItem
  }

}
</script>

<style scoped>
.about--subgrid {
  height: 100%;
  position: relative;
  z-index: 50;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 4fr 5fr 5fr;
}

.focus-area--title--outer {
  height: 100%;
  padding: .5rem 2rem;
}
.focus-area--title--inner {
  font-family: 'Aclonica', sans-serif;
  font-size: 320%;
  font-weight: normal;
  color: var(--offWhite);
}

.focus-area--text-one--outer {  
  margin: 1rem 2rem;
  padding: .75rem 2rem .75rem 1.5rem;
  background: linear-gradient(112.86deg, #DA0000 5.02%, rgba(137, 19, 28, 0) 88.06%);
  border-radius: 25px 0px 0px 25px;
}
.focus-area--text-one--inner {
  font-size: 1.85rem;
  font-weight: 300;
  color: var(--offWhite);
}

.focus-area--text-two--outer {  
  margin: 1rem 2rem;
  padding: .75rem 8rem .75rem 1.5rem;
  background: linear-gradient(112.86deg, #DA0000 5.02%, rgba(137, 19, 28, 0) 88.06%);
  border-radius: 25px 0px 0px 25px;
}
.focus-area--text-two--inner {
  font-size: 1.85rem;
  color: var(--offWhite);
}
</style>
