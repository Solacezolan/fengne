<template>
  <div class="navSwipe">
     <mt-swipe class="mintSwipe"  :auto="4000">
      <mt-swipe-item><img src="../../static/images/banner0@1x.jpg"></mt-swipe-item>
      <mt-swipe-item><img src="../../static/images/banner1@1x.jpg"></mt-swipe-item>
      <mt-swipe-item><img src="../../static/images/banner2@1x.jpg"></mt-swipe-item>
    </mt-swipe>
  </div>
</template>
<script>
 export default {
 data () {
  return {

  }
 }
 }
</script>
<style lang="scss" scoped="" type="text/css">
  .navSwipe{
    height: 1.2rem;
    .mintSwipe{
      width: 100%;
      height: 100%;
      img{display: block;outline: none;border:0;height: 100%;width: 100%;}
      
    }
  }
</style>
