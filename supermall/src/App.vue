<template>
  <div id="app">
    <!-- qq 756898435 dev-->
    <keep-alive exclude="Detail">
      <router-view></router-view>
    </keep-alive>
    <main-tab-bar/>
  </div>
</template>

<script>
  import MainTabBar from 'components/content/mainTabbar/MainTabBar'
  export default {
    name: 'app',
    components: {
      MainTabBar
    }
}
</script>

<style>
  @import 'assets/css/base.css'
</style>
