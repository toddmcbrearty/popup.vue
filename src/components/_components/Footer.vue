<template>
  <footer class="footer">
    <div class="container">
      <div class="content has-text-centered">
        <div class="columns">
          <div class="column">
            <div class="column-title">Column 1</div>
          </div>

          <div class="column">
            <div class="column-title">Column 2</div>
          </div>

          <div class="column">
            <div class="column-title">Column 2</div>
          </div>
        </div>
      </div>
    </div>
    <div class="has-text-centered has-text-left-mobile">
      <Copyright></Copyright>
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

  .footer {
    background: #d0d0d0;
  }
</style>
