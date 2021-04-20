<template>
  <div id="app">
    <router-view></router-view>
    <mainbar></mainbar>
  </div>
</template>
<script>
  import mainbar from 'components/content/mainbar/mainbar';
  export default {
    name: 'app',
    components: {
      mainbar
    }
  }
</script>
<style scoped>
  @import 'assets/css/base.css';
</style>
