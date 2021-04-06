<template lang="html">
  <div id="selected_country">
    <h2> Country Name: </h2>
    <h1>{{selectedCountry.name}}</h1>
    <p> Population:  </p>
    <p>  {{selectedCountry.population}} </p>
    <img v-bind:src="selectedCountry.flag" class="lrg-flag" />

    <neighbouring-countries>
    </neighbouring-countries>

</div>
</template>

<script>
import NeighbourCountry from './NeighbourCountry.vue';
export default {
  name: 'country-detail',
  props: ['selectedCountry'],
  components: {
    'neighbouring-countries': NeighbourCountry
  }
  
  
}
</script>

<style lang="css" scoped>

.lrg-flag {
  height: 100px
}

</style>
