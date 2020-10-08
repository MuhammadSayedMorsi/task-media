<template>
  <v-card
    class="card__blog"
    max-width="450"
  >
    <v-img
      src="https://cdn.vuetifyjs.com/images/cards/house.jpg"
      :aspect-ratio="16/9"
    >
    </v-img>
    <v-card-title>
      <div class="display-1 mb-2">
        <p class="par">Title video lorem ipsum dolor sit amet lorem ipsum dolor sit amet lorem ipsum dolor…</p>
      </div>
      <!-- <div class="title font-weight-regular grey--text">
        Monday, 12:30 PM, Mostly Sunny
      </div> -->
    </v-card-title>

    <v-row
      class="px-4"
      align="center"
    >
      <v-avatar
        size="24"
        class="mr-4"
        >
        <v-img
          :src="star"
          contain
        ></v-img>
      </v-avatar>

      <span class="n__views">4.5 . 43 views</span>

      <span class="premium">Premium</span>

      <span class="heart">18</span>
    </v-row>
  </v-card>
</template>

<script>
  import star from '../assets/star.svg'
  // import heart from '../assets/heart.svg'
export default {
  data: function () {
    return {
      star: star
    }
  }
}
</script>


<style lang="sass" scoped>
  .card__blog
    margin-bottom: 30px
    margin-top: 30px
    .par
      font-size: 18px
      font-weight: 900
      @media (max-width: 767px)
        font-size: 14px
        line-height: 1.5
    .n__views
      font-size: 16px
      font-weight: bold
    .premium
      width: 81px
      height: 24px
      background-color: #FDF2E8
      margin-left: 50px
      margin-right: 50px
      border-radius: 15px
      font-size: 14px
      text-align: center
      line-height: 24px
      @media (max-width: 767px)
        margin-left: 0
        margin-right: 0

    .heart
      width: 61px
      height: 31px
      background-color: #EF3F3F
      border-radius: 15px
      font-size: 14px
      text-align: right
      line-height: 31px
      padding-right: 10px
      position: relative
      &::before
        position: absolute
        bottom: 8px
        left: 10px
        content: ''
        background-image: url('../assets/heart.svg')
        width: 14px
        height: 14px
.v-image__image--cover
  border-radius: 30px
.v-sheet.v-card:not(.v-sheet--outlined)
  box-shadow: none

</style>