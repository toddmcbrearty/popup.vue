<template>
  <div class="date">
    <span v-html="copy"></span>
    <span v-text="copyDate"></span>
  </div>
</template>

<script>
  export default {
    name: "Copyright",

    data() {
      return {
        copy: '&copy;'
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

</style>
