<template>
  <div id="app">
    <Header></Header>

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

  export default {
    name: 'app',

    components: {
      Header,
      Content,
      Footer,
    },

    data() {
      return {
      }
    }
  }
</script>

<style lang="scss">
  @import 'scss/main';
</style>
