<template>
  <section class="header hero is-primary">
    <div class="hero-body">
      <div class="container">
        <h1 class="title" v-text="name"></h1>
        <h2 class="subtitle" v-show="showHeadline" v-text="headline"></h2>
      </div>
    </div>
  </section>
</template>

<script>
  export default {
    name: "Header",

    props: {
      name: {
        type: String,
        default: "Default",
      },
      headline: {
        type: String,
        default: "Default headline text",
      },
    },

    data() {
      return {
        showHeadline: {
          type: Boolean,
          value: this.headline !== '',
        },
      };
    },
  };
</script>

<style lang="scss">
  @import '../../scss/overrideables';

  .header {
    font-family: $secondaryFont;
  }

  .header .title, .header .subtitle {
    color: #000 !important;
  }

</style>
