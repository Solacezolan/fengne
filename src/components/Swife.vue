<template>
 <p>
 <mt-swipe :auto="2000">
  <mt-swipe-item v-for="item in items" :key="item.id">
  <a :href="item.href" rel="external nofollow" >
   <img :src="item.url" class="img"/>
   <span class="desc"></span>
  </a>
  </mt-swipe-item>
 </mt-swipe>
 </p>
</template>
<script>
 export default {
 data () {
  return {
  items: [{
   title: '你的名字',
   href: 'http://google.com',   url: 'http://localhost:8080/static/img1.png'
  }, {
   title: '我的名字',
   href: 'http://baidu.com',   url: 'http://localhost:8080/static/img2.png'
  }]
  }
 }
 }
</script>
<style>
	.imageBox{
		height: 3.12rem;
		.swiper-slide{
			margin: 0;
		}
	}
	img{
		width: 100%;
		height: 3.12rem;
	}
</style>
