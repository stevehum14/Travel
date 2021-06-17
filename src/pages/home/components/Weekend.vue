<template>
  <div>
    <div class="title">周末去哪儿</div>
    <ul>
      <li class="item border-bottom"
        v-for="item of list"
        :key="item.id"
      >
        <div class="item-img-wrapper">
          <img class="item-img" :src="item.imgUrl" />
        </div>
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
        </div>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  name: 'HomeWeekend',
  props: {
    list: Array
  },
  data () {
    return {
      // list: [{
      //   id: '0001',
      //   imgUrl: 'https://imgs.qunarzz.com/vs_ceph_vcimg/79faa5a73731e84a7731db49d5baa91e.jpeg',
      //   title: '古龙峡漂流',
      //   desc: '广东漂流看清远，清远漂流看古龙'
      // }, {
      //   id: '0002',
      //   imgUrl: 'https://imgs.qunarzz.com/vs_ceph_vcimg/79faa5a73731e84a7731db49d5baa91e.jpeg',
      //   title: '古龙峡漂流',
      //   desc: '广东漂流看清远，清远漂流看古龙'
      // }, {
      //   id: '0003',
      //   imgUrl: 'https://imgs.qunarzz.com/vs_ceph_vcimg/79faa5a73731e84a7731db49d5baa91e.jpeg',
      //   title: '古龙峡漂流',
      //   desc: '广东漂流看清远，清远漂流看古龙'
      // }, {
      //   id: '0004',
      //   imgUrl: 'https://imgs.qunarzz.com/vs_ceph_vcimg/79faa5a73731e84a7731db49d5baa91e.jpeg',
      //   title: '古龙峡漂流',
      //   desc: '广东漂流看清远，清远漂流看古龙'
      // }, {
      //   id: '0005',
      //   imgUrl: 'https://imgs.qunarzz.com/vs_ceph_vcimg/79faa5a73731e84a7731db49d5baa91e.jpeg',
      //   title: '古龙峡漂流',
      //   desc: '广东漂流看清远，清远漂流看古龙'
      // }]
    }
  }
}
</script>
<style lang="stylus" scoped>
@import '~styles/mixins.styl'
.title
  line-height: .8rem
  background: #eee
  text-indent: .2rem
.item-img-wrapper
  overflow: hidden
  height: 0
  padding-bottom:37.09%
  .item-img
    width: 100%
.item-info
  padding: .1rem
  .item-title
    line-height: .54rem
    font-size: .32rem
    ellipsis()
  .item-desc
    line-height: .4rem
    color: #ccc
    ellipsis()
</style>
