<template>
  <div id="app">
    <Header :name="shared.name" :headline="shared.headline"></Header>

    <Banner v-html="shared.bannerText" v-show="showBanner" background="is-success"></Banner>

    <Content v-html="shared.slotText"></Content>

    <Footer v-show="shared.showFooter" :shared="shared"></Footer>
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
    },

    computed: {
      showBanner() {
        return (this.shared.showBanner && this.shared.bannerText !== undefined && this.shared.bannerText !== '');
      }
    }
  }
</script>

<style lang="scss">
  @import 'scss/main';
</style>
