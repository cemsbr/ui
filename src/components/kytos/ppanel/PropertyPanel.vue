<template>
  <div :id="id" class="kytos-property-panel">
  <table>
      <slot />
  </table>
  </div>
</template>

<script>
import KytosBase from '../base/KytosBase.vue';

export default {
  name: 'kytos-property-panel',
  mixins: [KytosBase],
}
</script>

<style lang="sass">

@import '../../../assets/styles/variables'

.kytos-property-panel
 color: $fill-text
 overflow: auto
 max-height: 250px
 text-align: left
 margin: 0 auto
 display: block
 padding: 0.5em 0 1em 0.3em

 table
  display: table
  width: 100%

</style>
