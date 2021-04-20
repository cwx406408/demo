<template>
  <div>
    <navibar>
      <img slot="left" src="~assets/img/navibar/back.svg" alt="">
      <!-- <img slot="center" src="~assets/img/navibar/.svg" alt=""> -->
      <h2 slot="center">主页</h2>
      <img slot="right" src="~assets/img/navibar/forward.svg" alt="">
    </navibar>
  </div>
</template>
<script>
import navibar from 'components/common/navibar/navibar.vue'
export default {
  components: { navibar },
  name: 'home'
}
</script>