<template>
  <div class="wrapcards">
    <div class="wrap_title">
      <h3>Promotions</h3>
    </div>
    <div class="wrap_cards">
      <v-card class="card_style" v-for="link in CardText" :key="link.id">
      <div class="content">
        <h4>{{ link.title }}</h4>
        <span>{{ link.subTitle }}</span>
        <button>{{ link.btnText }}</button>
        <img :src="link.avatar"  alt="card_man_photo" />
      </div>
    </v-card>
    </div>
  </div>
</template>
<script>
// import CardMan from ''
export default {
  data: function () {
    return {
      // CardMan: CardMan,
      CardText: [
        { title: 'card one should be here', subTitle:'Lorem ipsum dolor sit amet', btnText: 'See now', avatar: require('@/assets/card_man.svg') },
        { title: 'card two should be here', subTitle:'Lorem ipsum dolor sit amet', btnText: 'See now', avatar: require('@/assets/card_2_avatar.svg')},
        { title: 'card three should be here', subTitle:'Lorem ipsum dolor sit amet', btnText: 'See now', avatar: require('@/assets/card_3_avatar.svg')},
        { title: 'card Four should be here', subTitle:'Lorem ipsum dolor sit amet', btnText: 'See now', avatar: require('@/assets/card_2_avatar.svg')}

      ]
    }
  }
}
</script>

<style lang="sass" scoped>
.wrapcards
  display: flex
  flex-direction: column
  .wrap_title
    h3
      margin-bottom: 23px
  @media (max-width: 992px)
    // flex-direction: column
    align-items: center

  .wrap_cards
    display: flex
    justify-content: space-between
    @media (max-width: 992px)
      flex-direction: column
      align-items: center

    .v-sheet.v-card:not(.v-sheet--outlined)
      box-shadow: none
    .theme--light.v-card
      background-color: #FF9638
    .card_style
      width: 296px
      height: 148px
      position: relative
      border-radius: 15px
      @media (max-width: 992px)
        margin-bottom: 20px
      .content
        display: flex
        align-items: flex-start
        flex-direction: column
        padding-top: 33px
        padding-left: 25px
        h4
          font-size: 16px
          color: #fff
          margin-bottom: 13px
        span
          font-size: 12px
          color: #fff
      button
        width: 71px
        height: 24px
        margin-top: 17px
        background-color: #fff
        border-radius: 5px
        bottom: 20px
        position: absolute
        transition: all 0.4s  ease

        &:hover
          bottom: 22px
          transition: all 0.4s  ease
      img
        position: absolute
        top: 0
        right: 0

</style>