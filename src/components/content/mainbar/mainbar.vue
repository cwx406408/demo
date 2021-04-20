<template>
  <div>
    <tabbar>
      <tabbaritem>
        <img src="~assets/img/tabbar/home.svg" alt="">
        <div>主页</div>
      </tabbaritem>
      <tabbaritem>
        <img src="~assets/img/tabbar/home.svg" alt="">
        <div>主页</div>
      </tabbaritem>
      <tabbaritem>
        <img src="~assets/img/tabbar/home.svg" alt="">
        <div>主页</div>
      </tabbaritem>
      <tabbaritem>
        <img src="~assets/img/tabbar/home.svg" alt="">
        <div>主页</div>
      </tabbaritem>
    </tabbar>
  </div>
</template>

<script>
import tabbar from 'components/common/tabbar';
import tabbaritem from 'components/common/tabbaritem';
import Tabbar from '../../common/tabbar.vue';
export default {
  name: 'mainbar',
  components: {
    tabbar,
    tabbaritem
  }
}
</script>
<style scoped>

</style>