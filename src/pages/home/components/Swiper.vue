<template>
  <div class="wrapper">
    <swiper :options="swiperOption" ref="mySwiper">
      <!-- slides -->
      <swiper-slide v-for="item of swiperList" :key="item.id">
        <img class='swiper-img' :src="item.imgUrl"/>
      </swiper-slide>
      <!-- Optional controls -->
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </div>
</template>

<script type="text/ecmascript-6">

  export default{
    name: 'HomeSwiper',
    data () {
      return {
        swiperOption: {
          pagination: '.swiper-pagination',
          loop: true
        },
        swiperList: [
          {
            id: '001',
            imgUrl: 'https://imgs.qunarzz.com/p/tts7/1805/51/8db4f954e22ca02.jpg_r_390x260x90_df87ae37.jpg'
          }, {
            id: '002',
            imgUrl: 'https://imgs.qunarzz.com/p/tts0/1806/6d/b776b0b2da64e502.jpg_r_390x260x90_550834a8.jpg'
          }
        ]
      }
    }
  }

</script>

<style lang="stylus" rel="stylesheet/stylus" scoped>
  .wrapper
    overflow hidden
    width 100%;
    height 0;
    padding-bottom 31.25%
    .swiper-img
      width 100%
</style>
