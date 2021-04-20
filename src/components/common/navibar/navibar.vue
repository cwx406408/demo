<template>
  <div class="navi-bar">
    <div class="left">
      <slot name="left"></slot>
    </div>
    <div class="center">
      <slot name="center"></slot>
    </div>
    <div class="right">
      <slot name="right"></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: 'navibar'
  // props: {
  //   BackgroundColor: {
  //     type: String,
  //     default: '#fff'
  //   }
  // },
  // computed: {
  //   bgColor () {
  //     return {backgroundColor: this.BackgroundColor}
  //   }
  // }
}
</script>
<style scoped>
  .navi-bar {
    display: flex;
    line-height: 44px;
    text-align: center;
    box-shadow: 0  1px 1px rgba(100,100,100,0.1);
  }

  .navi-bar img {
    height: 24px;
    width: 24px;
    vertical-align: middle;
  }

  .left .right {
    width: 60px;
  }

  .center {
    flex: 1;
  }
</style>
