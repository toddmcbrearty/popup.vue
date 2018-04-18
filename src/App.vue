<template>
  <div id="app">
    <Header :name="shared.name" :headline="shared.headline"></Header>

    <Content>
      <div slot="content">
        This is the content
      </div>
    </Content>

    <Footer></Footer>
  </div>
</template>

<script>
  import Header from './components/Header';
  import Content from './components/Content';
  import Footer from './components/Footer';
  import Settings from './settings';

  export default {
    name: 'app',

    components: {
      Header,
      Content,
      Footer,
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
