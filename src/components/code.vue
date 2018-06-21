<template>
	<div class="code" :class="borderType">
		<div class="pinnerLeft">
			<h3>{{content.title}}</h3>
			<div class="labelDetail">
				{{content.messaage}}
			</div>
			<div v-if="content.detail!=null&&content.detail!=''">
				{{content.detail}}
			</div>
		</div>
		<div class="pinnerRight">
			<img :src="content.src"/>
		</div>
		</div>	 
	<div>
</template>
<script >
	name:"code",
	props:{
		content:{
			type:Object,
			required: true
		},
		borderType:{
			type:String
		}
	}
</script>
<style lang="scss" scoped="" type="text/css">
	

</style>