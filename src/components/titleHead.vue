<template lang="html">
	<div class="header_title">
		<a class="header_url lf" @click="gotoBack()"> <i class="iconfont icon-fanhui"></i></a>
		 <slot>
  		 </slot>
		<h2>{{title}}</h2>
	</div>
</template>

<script>

export default {
	props:["title"],
	name:'titleHead',
	methods : {
		gotoBack:function(){
			this.$router.go(-1);
		}
	}
}
</script>

<style lang="scss" scoped="" type="text/css">
	.header_title{
		height: 0.45rem;
		width: 100%;
		line-height: 0.45rem;
		text-align: center;
		border-bottom: 1px solid #ddd;
		.register{
			color: #328CCC;
		}
		.header_url{
			width: 0.6rem;
			font-size: 0.14rem;
			height: 0.45rem;
			line-height: 0.45rem;
			i{
				color: #328CCC;
			}
		}
		h2{
			width: 60%;
			margin:0 auto;
			font-weight: bold;
			font-size: 0.14rem;
		}
	}
</style>