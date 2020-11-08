/* eslint-disable */
<template>
    <div id="app">
    <router-view/><!--是上面的路由部分-->
      <FooterGuide v-show="$route.meta.showFooter"/><!--下面的底部导航部分,用v-show来实现是否显示-->
    </div>
</template>

<script>
  import FooterGuide from './components/FooterGuide/FooterGuide'
export default {
    components:{
      FooterGuide
    }
}
</script>

<style lang="stylus" rel="stylesheet/stylus">
  #app {
    width: 100%;
    height: 100%;
    background: #f5f5f5;
    position: relative;
  }
</style>
