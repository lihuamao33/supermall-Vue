<template>
  <div class="nav-bar">
      <div class="left"><slot name="left"></slot></div>
      <div class="center"><slot name="center"></slot></div>
      <div class="right"><slot name="right"></slot></div>
  </div>
</template>
<script>
export default {
  name: 'NavBar',
  data () {
   return {}
  },
   methods:{}
}
</script>
<style scoped>
  .nav-bar {
      display:flex;
      line-height:44px;/* 一般上部导航为44 */
      text-align: center;
      box-shadow: 0 1px 1px rgb(100,100,100,.1);
  }
  .left, .right {
      width: 60px;
  }
  .center {
      flex:1;
  }
</style>