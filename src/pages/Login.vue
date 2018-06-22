<template lang="html">
	<div>
		<title-head title="登录">
			<router-link class="header_url register rt" :to="{}"><router-link to="/register">注册</router-link></router-link>
		</title-head>
		<div class="submitBox">
			<form>
				<div class="account">
					<label for="account" class="lf">账号</label>
					<input type="text" name="account" v-model="account" placeholder="请输入账号" />
				</div>
				<div class="passwords">
					<label class="lf" for="password">密码</label>
					<input type="password" name="password" v-model="confirmwords" placeholder="请输入密码" />
				</div>
				<p><span class="filelogin lf">无法登录？</span><span class="forgetword rt">忘记密码？</span></p>
			</form>
			<input type="submit" class="button" value="确定"/>
		</div>
	</div>
</template>

<script>
import titleHead from '../components/titleHead.vue'
export default {
	name:'login',
	data(){
		return{
			account:"",
			passwords:"",
			confirmwords:""
		}
	},
	components: {
	   titleHead
  	}
}
</script>

<style lang="scss" scoped="" type="text/css">
	.submitBox{
		form{
			width: 100%;
			padding-left: 0.1rem;
			margin-top: 0.2rem;
			div{
				height: 0.45rem;
				line-height: 0.45rem;
				width: 100%;
				float: left;
				label{
					width: 20%;
					height: 0.45rem;
					line-height: 0.45rem;
					text-align: center;
					display: inline-block;
					float: left;
					color: #328CCC;
				}
				input{
					width: 80%;
					float: left;
					box-sizing: border-box;
	    			height: 0.45rem;
				}
			}
			p{
				width: 100%;
				margin:  0.1rem 0 0 0;
				clear: both;
				float: left;
				span{
					width: 30%;
					display: inline-block;
					font-size: 0.12rem;
					text-align: center;
				}
			}
		}
		input.button{
				width: 90%;
				margin: 0 auto;
				height: 0.4rem;
				line-height: 0.4rem;
				margin: 0.15rem 0 0 0;
				background: #328CCC;
				margin-left: 5%;
				color: #fff;
				cursor: pointer;
				border-radius: 2px;
			}
	}
</style>