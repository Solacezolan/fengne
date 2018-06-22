<template lang="html">
  <div class="Header">
      <div class="navbar">长沙<i class="iconfont icon-xiangxia"></i></div>
      <div class="searchBox">
        <i class ="iconfont icon-sousuo"></i>
        <input class="searchInput" type="text"  readonly="readonly" placeholder="请输入景区/地名" name="search" value=""/>
      </div>
      <div class="navbar" @click="toLogin">登录</div>
  </div>
</template>

<script>
  
export default {
  name:'heades',
    methods: { 
    toLogin:function(){
      this.$router.push('/login');
    },
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
  .Header{
    height: 0.4rem;
    line-height: 0.4rem;
    color: #fff;
    background: #328CCC;
    .searchBox{
      width:60%;
      float: left;
      position: relative;
      i{
        font-size: 0.213rem;
        position: absolute;
        top: 0.01rem;
        left: 0.106rem;
      }
      input{
        height: 0.25rem;
        line-height: 0.25rem;
        width: 100%;
        border: none;
        outline: none;
        box-sizing: border-box;
        background: $backgroundSmall;
        padding-left: 0.4rem;
      }
      .searchInput::-webkit-input-placeholder {
            color: #fff;
         }
    }
    .navbar{
      width:20%;
      float: left;
      height: 100%;
      text-align: center;
      .icon-xiangxia{
        font-size:0.15rem;
        margin-left:0.066rem;
        vertical-align: middle;
      }
    }
  }
</style>
