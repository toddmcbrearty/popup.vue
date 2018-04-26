<template>
  <div class="date">
    <span v-html="preText"></span>
    <span v-html="copy"></span>
    <span v-text="copyDate"></span>
  </div>
</template>

<script>
  export default {
    name: "Copyright",

    props: ['preText'],

    data() {
      return {
        copy: '&copy;',
      }
    },

    computed: {
      copyDate() {
        return new Date().getFullYear();
      }
    },
  }

</script>

<style scoped>
  .date {}
</style>
