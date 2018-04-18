<template>
  <div id="app">
    <Header :name="shared.name" :headline="shared.headline"></Header>

    <Banner :banner-text="shared.banner"></Banner>

    <Content>this is slot text</Content>

    <Footer></Footer>
  </div>
</template>

<script>
  import Header from './components/_components/Header';
  import Content from './components/_components/Content';
  import Footer from './components/_components/Footer';
  import Banner from './components/_components/Banner';
  import Settings from './settings';

  export default {
    name: 'app',

    components: {
      Header,
      Content,
      Footer,
      Banner,
    },

    data() {
      return {
        shared: Settings
      }
    }
  }
</script>

<style lang="scss">
  @import 'scss/main';
</style>
