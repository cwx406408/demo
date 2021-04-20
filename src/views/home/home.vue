<template>
  <div>
    <navibar>
      <img slot="left" src="~assets/img/navibar/back.svg" alt="">
      <!-- <img slot="center" src="~assets/img/navibar/.svg" alt=""> -->
      <h2 slot="center">主页</h2>
      <img slot="right" src="~assets/img/navibar/forward.svg" alt="">
    </navibar>
    <div>
      <img :src="this.data.img" alt="">
    </div>
    
  </div>
</template>
<script>
import navibar from 'components/common/navibar/navibar.vue'
import {request} from 'network/request.js'
export default {
  components: { navibar },
  name: 'home',
  data() {
    return {
      data: {}
    }
  },
  created() {
    //console.log('created');
    request({
      url: '/api/data'
    }).then((result) => {
      this.data = result.data
      //console.log(this.data);
    }).catch((err) => {
      console.log(err);
    });
  }
}
</script>

