<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App',
  created() {
    this.$store.commit('INIT_STATE', '');
  },
}
</script>

<style lang="scss">
  @import 'src/assets/css/reset';
  @import 'src/assets/css/common';

  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    height: 100%;
  // overflow: hidden;
    /*text-align: center;
    color: #2c3e50;
    margin-top: 60px;*/
  }
</style>
