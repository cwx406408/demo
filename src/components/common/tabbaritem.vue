<template>
  <div class="tabbaritem" @click="itemClick">
    <div v-if="!IsActive">
      <slot name="item-icon"></slot>
    </div>
    <div v-else>
      <slot name="item-icon-active"></slot>
    </div>
    <div :style="Color">
      <slot name="item-text"></slot>
    </div>
  </div>
</template>
<script>
export default {
  name: 'tabbaritem',
  computed: {
    Color () {
      if(this.$route.path == this.path){
        return {color: this.activeColor}
      }

      return {color: this.inactiveColor}
    },
    IsActive () {
      return this.$route.path == this.path
    }
  },
  methods: {
    itemClick () {
      if (this.$route.path != this.path){
        this.$router.push(this.path)
      }
      
      return
    }
  },
  props: {
    path: {
      type: String,
      default: ''
    },
    activeColor: {
      type: String,
      default: '#ff0000'
    },
    inactiveColor: {
      type: String,
      default: '#000000'
    }
  }
}
</script>
<style scoped>
  .tabbaritem {
    flex: 1;
    text-align: center;
    height: 49px;
    font-size: 14px;
  }

  .tabbaritem img{
    height: 24px;
    width: 24px;
    margin-top: 3px;
    vertical-align: middle;
    margin-bottom: 3px;
  }
</style>