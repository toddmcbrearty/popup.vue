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
    font-size: 2rem;
    font-weight: 700;
  }
</style>
