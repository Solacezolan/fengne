<template>
  <div id="app">
    <transition :name="LoadDirection">
      <router-view></router-view>
    </transition>
  </div>
</template>

<script>
export default {
  name: 'App',
  data:{
    return(){
      LoadDirection:"right"
    }
  }
}
</script>

<style lang="scss" scoped="">
    
</style>
