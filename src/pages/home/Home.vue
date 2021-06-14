<template>
  <div>
    <home-header></home-header>
    <Home-swiper></home-swiper>
    <Home-icons></home-icons>
  </div>
</template>
<script>
import HomeHeader from './components/Header.vue'
import HomeSwiper from './components/Swiper'
import HomeIcons from './components/Icons'
export default {
  name: 'Home',
  components: {
    HomeHeader: HomeHeader,
    HomeSwiper: HomeSwiper,
    HomeIcons: HomeIcons
  }
}
</script>
<style></style>
