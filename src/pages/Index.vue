<template>
  <div class="app">
  	<Header></Header>
  	<swife></swife>
  </div>
</template>

<script>
import Header from '../components/Header.vue'
import Swife from '../components/Swife.vue'
export default {
  name: 'index',
  components: {
  	Header,
  	Swife
  },
  data () {
    return {
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
h1, h2 {
  font-weight: normal;
  background: $background;
  font-size: $font-size;
  height: 2rem;

}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
#app  .app{
	width: 100%;
}
.demo-grid{
     background: $background;
}
.serve{
	height: 1.6rem;
	background: #fff;
	margin: 0.266rem;
		.col{
			padding: 0.266rem 0.4rem;
		}
		.muicon{
			border-right: 1px solid #DDDDDD;
		}
		.pinnerLeft{
			width: 70%;
			float: left;
			height: 100%;
			h3{
				margin: 0 0 0.1rem 0;
				height: 0.3rem;
				line-height: 0.3rem;
				text-align: left;
				font-size:0.24rem;
			}
			.labelDetail{
				height: 0.534rem;
				width: 100%;
				margin: 0;
				padding: 0;
				word-break: break-word;
				line-height: 0.2933rem;
				text-align: left;
				font-size:0.2133rem;
				color: #333;
			}
		}
		.pinnerRight{
			width: 30%;
			float: right;
			height: 100%;
			img{
				width: 100%;
				height: 100%;
			}
		}
	
	
}
.remmade{
	border-top: 1px solid #ddd;
	border-bottom: 1px solid #ddd;
	margin: 0.2rem 0;
	.muicon{
		height: 0.533rem;
		line-height: 0.533rem;
		i{
			color: #FCAA00;
			font-size: 0.4266rem;
		}
	}
	.muremmade{
		b{
			width: 1px;
			height: 0.266rem;
			position: absolute;
			background: #ddd;
			left: 0;
			top:0.133rem;
		}
		i{
			position: absolute;
			color: #ddd;
			right: 0.1333rem;
			top:0;
			font-size: 0.2933rem;
		}
		padding-left:0.266rem;
		position:relative;
		text-align: left;
		height: 0.533rem;
		line-height: 0.533rem;
		color:#FCAA00;
		cursor:pointer;
		span{
			font-weight: bold;
		}
	}
}
</style>
