<template>
  <footer class="footer">
    <div class="container">
      <div class="content has-text-centered">
        <div class="columns">
          <div class="column is-two-fifths">
            <div class="has-text-center column-title">Column 1</div>
            <Copyright></Copyright>
          </div>

          <div class="column is-offset-one-fifth">
            <div class="has-text-center column-title">Column 2</div>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
  import Copyright from './Copyright';

  export default {
    name: "Footer",

    components: {
      Copyright
    }
  }
</script>

<style lang="scss">
  .column-title {
    border-bottom: 1px solid #4a4a4a;
  }
</style>
