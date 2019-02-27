<template>
  <div 
    class="grid--item--outer" 
    :style="{ 'grid-area': gridArea }">
    <slot default></slot>
    <slot name="secondary"></slot>
  </div>
</template>

<script>
export default {
  props: ['gridArea']
}
</script>

<style>

</style>
