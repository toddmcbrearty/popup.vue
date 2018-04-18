<template>
    <div class="main content">
      <slot name="content"></slot>
    </div>
</template>

<script>
  export default {
    name: "Content"
  }
</script>

<style lang="scss">
  .main {
    flex: 1;
    padding: 1em;
  }
</style>
