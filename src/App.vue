<template>
  <v-app>
      <Nav />
    <v-main class="px-16">
      <Content />
      <Items />
      <ButtonList />
      <CardBlog/>
    </v-main>
  </v-app>
</template>

<script>
import Nav from './components/Nav';
import Content from './components/Content'
import Items from './components/Items'
import ButtonList from './components/ButtonList'
import CardBlog from './components/CardBlog'



export default {
  name: 'App',

  components: {
    Nav,
    Content,
    Items,
    ButtonList,
    CardBlog
  },

  data: () => ({
    //
  }),
};
</script>
