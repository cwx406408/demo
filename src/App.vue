<template>
  <div id="app">
    <keep-alive>
      <router-view></router-view>
    </keep-alive>
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
