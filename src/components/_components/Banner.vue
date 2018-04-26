<template>
  <div class="banner notification has-text-centered"
       :class="background">
    <slot></slot>
  </div>
</template>

<script>
  export default {
    name: "Banner",

    props: {
      background: {
        type: String,
        default: 'is-info'
      }
    }
  };
</script>

<style lang="scss">
  .banner.notification {
    font-size: 1.75rem;
    padding-top: 0.2em;
    padding-bottom: 0.2em;
    color: #495e91;
  }
</style>
