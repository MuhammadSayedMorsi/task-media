<template>
    <Card class="wrapper__cards"/>
</template>

<script>

import Card from './Card'

export default {
  name: 'App',

  components: {
    Card
  },

  data: () => ({
    //
  }),
};
</script>

<style lang="sass" scoped>
  .wrapper__cards
    margin-top: 85px
</style>