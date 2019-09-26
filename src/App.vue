<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
    export default {
        components: {}
    }
</script>
<style lang="scss">
  *{
    margin: 0;
    padding: 0;
  }
  html{
    font-size: 26.67vw;
  }
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    font-size: .14rem;
  }
</style>