<template>
  <div class="notification has-text-centered"
       :class="background"
       v-html="bannerText"
       v-if="bannerText !== ''"></div>
</template>

<script>
  export default {
    name: "Banner",

    props: {
      bannerText: {
        type: String,
        default: '',
      },

      background: {
        type: String,
        default: 'is-warning'
      }
    }
  };
</script>

<style scoped>

</style>
