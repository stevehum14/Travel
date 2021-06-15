<template>
  <div>
    <home-header></home-header>
    <Home-swiper></home-swiper>
    <home-icons></home-icons>
    <home-recommend></Home-recommend>
  </div>
</template>
<script>
import HomeHeader from './components/Header.vue'
import HomeSwiper from './components/Swiper'
import HomeIcons from './components/Icons'
import HomeRecommend from './components/Recommend'
export default {
  name: 'Home',
  components: {
    HomeHeader: HomeHeader,
    HomeSwiper: HomeSwiper,
    HomeIcons: HomeIcons,
    HomeRecommend: HomeRecommend
  }
}
</script>
<style></style>
