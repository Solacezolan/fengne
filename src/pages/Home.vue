<template>
  <div class="app">
  	<Header></Header>
  	<swife></swife>
  	<div class="moduleBox">
	  	<div class="modules">
		    <div class="modules_items">
		    	<div>
		    		<i style="color: #DD5144;" class="iconfont icon-jian"></i>
		    	</div>
		    	<p>热门推荐</p>
		    </div>
		    <div class="modules_items">
		    	<div>
		    		<i style="color: #328ccc;"  class="iconfont icon-jingwaizijia"></i>
		    	</div>
		    	<p>境外景点</p>
		    </div>
		    <div class="modules_items">
		    	<div>
		    		<i style="color: #2EA7E0;"  class="iconfont icon-jingnei"></i>
		    	</div>
		    	<p>境内景点</p>
		    </div>
		    <div class="modules_items">
		    	<div>
		    		<i style="color:#C568EC;"  class="iconfont icon-jiudian1"></i>
		    	</div>
		    	<p>酒店/旅馆</p>
		    </div>
		  </div>
		  <div class="modules">
		     <div class="modules_items">
		     	<div>
		     		<i style="color:#33A3E5 ;"  class="iconfont icon-jipiao1"></i>
		     	</div>
		     	<p>火车票/机票</p>
		     </div>
		    <div class="modules_items">
		    	<div>
		    		<i style="color:#C1A108 ;"  class="iconfont icon-meishi1"></i>
		    	</div>
		    	<p>美食/特产</p>
		    </div>
		    <div class="modules_items">
		    	<div>
		    		<i style="color:#BBBEC1;"  class="iconfont icon-gonglve"></i>
		    	</div>
		    	<p>旅游攻略</p>
		    </div>
		    <div class="modules_items">
		    	<div>
		    		<i style="color:#1091FF ;"  class="iconfont icon-gengduogongneng1"></i>
		    	</div>
		    	<p>更多功能</p>
		    </div>
		  </div>
	  </div>
  	<div class="exclusive">
   		<div gutter>
    		<div class="exclusiveLeft" >
    			<i class="iconfont icon-tuijian"></i>
    		</div>
    		<div  class="exclusiveRight">
    			<i class="iconfont icon-xiangyou"></i>
    			<span>登录</span> 
    			 查看专属推荐
    		</div>
  		</div>
   	</div> 
  </div>
</template>

<script>
import Header from '../components/Header.vue'
import Swife from '../components/Swife.vue'
import codes from '../components/codes.vue'
export default {
  name: 'index',
  components: {
  	Header,
  	Swife,
  	codes
  },
  data () {
  	
    return {
		items:{
			title:"asdasdasd"
		}
    }
  },
   methods: {

  },
  mounted:function() {
	}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped="" type="text/css">
.moduleBox{
	border-bottom: 1px solid #ddd;
	float: left;
	width: 100%;
	.modules{
		float: left;
		width: 100%;
		.modules_items{
			float: left;
			width: 25%;
			text-align: center;
			height: 0.8rem;
			div{
				height: 0.4rem;
				margin: 0.1rem 0 0.05rem 0;
				vertical-align: middle;
				.iconfont{
					font-size: 0.36rem;
				}
				
			}
			p{
					font-size: 0.12rem
			}
		}
	}
}
.exclusive{
	border-bottom: 1px solid #ddd;
	float: left;
	width: 100%;
	.exclusiveLeft{
		float: left;
		width: 10%;
		text-align: center;
		height: 0.35rem;
		line-height: 0.35rem;
		i{
			color: #FCAA00;
			font-size: 0.25rem;
		}
	}
	.exclusiveRight{
		float: left;
		font-size: 0.12rem;
		width: 90%;
		box-sizing: border-box;
		
		i{
			position: absolute;
			color: #ddd;
			right: 0.1333rem;
			top:0;
			
		}
		span{
			color: #fcaa00;
		}
		padding-left:0.1rem;
		position:relative;
		text-align: left;
		height: 0.35rem;
		line-height: 0.35rem;
		
		cursor:pointer;
		span{
			font-weight: bold;
		}
	}
}

</style>
