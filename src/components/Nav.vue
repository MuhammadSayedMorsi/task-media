<template>
  <div class="wrapper_nav">
    <v-app-bar
      color="white"
      class="custome_color  paddin_space">
      <v-toolbar-title class="Logo">Logo</v-toolbar-title>

      <v-spacer></v-spacer>
      <div class="wrap__button_nave">
        <button class="consult_btn">
        <img :src="headphone" alt="headphone_icon">
        Consultaion
        </button>

        <button>
          <img :src="messangerIcons" alt="consult">
        </button>

        <button>
          <img :src="ring" alt="">
        </button>

        <button class="per_btn">
          <img :src="person" alt="">
        </button>
      </div>
    </v-app-bar>
  </div>
</template>
<script>
import headphone from '../assets/headphone.svg'
import messangerIcons from '../assets/messangerIcons.svg'
import ring from '../assets/ring.svg'
import person from '../assets/person.svg'
  export default {
    name: 'HelloWorld',

    data: function () {
      return {
        headphone: headphone,
        messangerIcons: messangerIcons,
        ring: ring,
        person: person
      }
    }
  }
</script>
<style lang="sass">
  .wrapper_nav
    .v-sheet.v-app-bar.v-toolbar:not(.v-sheet--outlined)
      box-shadow: 0px 2px 4px -1px #BDBEBF, 0px 4px 5px 0px #BDBEBF, 0px 1px 10px 0px #BDBEBF
    .Logo
      position: relative
      width: 100px
      &::after
        content: ''
        position: absolute
        top: 12px
        bottom: 0
        right: 44px
        width: 10px
        height: 10px
        border-radius: 10px
        background-color: #DE7143
    .consult_btn
      width: 141px
      height: 34px
      border-radius: 34px
      background-color: #EFEFFD
      display: flex
      justify-content: space-evenly
      align-items: center
    button
      border: 0
      outline: none
    .per_btn
      background-color: #EFEFFD
      width: 40px
      height: 40px
      border-radius: 40px
      display: flex
      justify-content: center
      align-items: center
    .wrap__button_nave
      width: 400px
      display: flex
      justify-content: space-between
    .paddin_space
      padding-left: 64px
      padding-right: 64px
      @media(max-width: 767px)
        padding: 0 !important
</style>