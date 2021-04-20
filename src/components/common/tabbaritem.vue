<template>
  <div class="tabbaritem">
    <slot></slot>
  </div>
</template>
<script>
export default {
  name: 'tabbaritem'
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