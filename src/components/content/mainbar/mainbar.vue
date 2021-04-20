<template>
  <div>
    <tabbar>
      <tabbaritem path="/home" active-color="#d81e06" inactive-color="#515151">
        <img slot="item-icon" src="~assets/img/tabbar/home.svg" alt="">
        <img slot="item-icon-active" src="~assets/img/tabbar/home_active.svg" alt="">
        <div slot="item-text">主页</div>
      </tabbaritem>
      <tabbaritem path="/category" active-color="#d81e06" inactive-color="#515151">
        <img slot="item-icon" src="~assets/img/tabbar/category.svg" alt="">
        <img slot="item-icon-active" src="~assets/img/tabbar/category_active.svg" alt="">
        <div slot="item-text">分类</div>
      </tabbaritem>
      <tabbaritem path="/cart" active-color="#d81e06" inactive-color="#515151">
        <img slot="item-icon" src="~assets/img/tabbar/cart.svg" alt="">
        <img slot="item-icon-active" src="~assets/img/tabbar/cart_active.svg" alt="">
        <div slot="item-text">购物车</div>
      </tabbaritem>
      <tabbaritem path="/profile" active-color="#d81e06" inactive-color="#515151">
        <img slot="item-icon" src="~assets/img/tabbar/profile.svg" alt="">
        <img slot="item-icon-active" src="~assets/img/tabbar/profile_active.svg" alt="">
        <div slot="item-text">我的</div>
      </tabbaritem>
    </tabbar>
  </div>
</template>

<script>
import tabbar from 'components/common/tabbar';
import tabbaritem from 'components/common/tabbaritem';
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