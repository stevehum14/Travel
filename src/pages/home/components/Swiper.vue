<template>
 <div class="wrapper">
  <swiper  :options="swiperOptions">
    <swiper-slide v-for="item of swiperList" :key="item.id">
    <img class="swiper-img" :src="item.imgUrl">
    </swiper-slide>
    <div class="swiper-pagination" slot="pagination"></div>
  </swiper></div>
</template>
<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOptions: {
        pagination: {
          el: '.swiper-pagination'
        },
        loop: true
      },
      swiperList: [{
        id: '0001',
        imgUrl: 'https://imgs.qunarzz.com/p/tts2/2101/6f/f5ff0112c2571402.jpg_750x440_2eb5e98e.jpg'
      }, {
        id: '0002',
        imgUrl: 'https://imgs.qunarzz.com/p/tts2/2101/82/2ab7013e03202702.jpg_750x440_8f306202.jpg'
      }]
    }
  }
}
</script>
<style lang="stylus" scoped>
.wrapper >>> .swiper-pagination-bullet-active
    background:#fff
.wrapper
    overflow:hidden
    width: 100%
    height:0
    padding-bottom:58.67%
    background:#eee
    .swiper-img
        width:100%
</style>
