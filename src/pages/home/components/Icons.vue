<template>
  <div class="icons">
    <div class="icon" v-for="item of iconList" :key="item.id">
      <!--<img class="icon-img" :src="item.imgUrl"/>-->
      <!--<div class="icon-desc">{{item.desc}}</div>-->1
    </div>
  </div>
</template>

<script type="text/ecmascript-6">
  export default{
    name: 'HomeIcons',
    data () {
      return {
        iconList: [{
          id: '0001',
          imgUrl: 'https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=2534684071,535927287&fm=11&gp=0.jpg',
          desc: '泡温泉'
        }, {
          id: '0002',
          imgUrl: 'https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=3455050251,4251828335&fm=26&gp=0.jpg',
          desc: '动植园'
        }, {
          id: '0003',
          imgUrl: 'https://ss0.bdstatic.com/70cFvHSh_Q1YnxGkpoWK1HF6hhy/it/u=3552344811,3180258313&fm=11&gp=0.jpg',
          desc: '景点门票'
        }, {
          id: '0004',
          imgUrl: 'https://t8.baidu.com/it/u=1753288051,1199067073&fm=191&app=48&size=h300&n=0&g=4n&f=JPEG?sec=1853310920&t=0cb049ffb1c610b27c76791bb75ba174',
          desc: '滑雪季'
        }, {
          id: '0005',
          imgUrl: 'https://ss0.bdstatic.com/70cFvHSh_Q1YnxGkpoWK1HF6hhy/it/u=723089232,2750708922&fm=26&gp=0.jpg',
          desc: '自然风光'
        }, {
          id: '0006',
          imgUrl: 'https://ss0.bdstatic.com/70cFvHSh_Q1YnxGkpoWK1HF6hhy/it/u=723089232,2750708922&fm=26&gp=0.jpg',
          desc: '景点门票'
        }, {
          id: '0007',
          imgUrl: 'https://ss0.bdstatic.com/70cFvHSh_Q1YnxGkpoWK1HF6hhy/it/u=723089232,2750708922&fm=26&gp=0.jpg',
          desc: '一日游'
        }, {
          id: '0008',
          imgUrl: 'https://ss0.bdstatic.com/70cFvHSh_Q1YnxGkpoWK1HF6hhy/it/u=723089232,2750708922&fm=26&gp=0.jpg',
          desc: '全部'
        }]
      }
    }
  }
</script>

<style lang="stylus" rel="stylesheet/stylus" scoped>
  .icons
    display grid
    grid-template-rows 100px 100px
    grid-template-columns repeat(4, 1fr);
    margin-top 10px;
    .icon
      box-sizing border-box
    .icon-img
      width 100px;
      height 80px;
      padding-left 10px;
      padding-right 10px;
      border-radius 60px;
    .icon-desc
      width 100%;
      line-height 20px;
</style>
