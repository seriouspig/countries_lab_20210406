<template lang="html">
  <div id="favourite_countries">
    <h2>Favourite Countries</h2>
    <p  v-for="country in favourite_countries"   :value="country" > {{country.name}}    </p>

  </div>
</template>

<script>
export default {
  name: 'favourite-countries',
  props: ['favourite_countries']
}
</script>

<style lang="css" scoped>
</style>
