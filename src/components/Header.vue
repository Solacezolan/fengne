<template lang="html">
  <div>
     	<mt-header title="标题过长会隐藏后面的内容啊哈哈哈哈">  
          <router-link to="/" slot="left">  
            <mt-button icon="back" @click="handleClose">返回</mt-button>  
          </router-link>  
          <mt-button icon="more" slot="right" @click="more"></mt-button>  
        </mt-header>  
  </div>
</template>

<script>
export default {
  name:'heades',
    methods: { 
  	handleClose: function(){  
        console.log("返回")  
    },  
    more: function(){  
        console.log("更多")  
    }  
  }
}
</script>

<style lang="scss" scoped="" type="text/css">
  .demo-grid{
    height: 0.533rem;
    line-height: 0.533rem;
    font-size:0.213rem;
    color: #fff;
    .searchBox{
      position: relative;
      i{
        font-size: 0.213rem;
        position: absolute;
        top: 0.01rem;
        left: 0.106rem;
      }
      input{
        height: 0.4rem;
        line-height: 0.4rem;
        width: 100%;
        border: none;
        outline: none;
        background: $backgroundSmall;
        padding-left: 0.4rem;
      }
      .searchInput::-webkit-input-placeholder {
            color: #fff;
         }
    }
    .navbar{
      .icon-xiangxia{
        font-size:0.15rem;
        margin-left:0.066rem;
        vertical-align: middle;
      }
    }
  }
</style>
