<template>
  <div class="wrapper">
    <swiper :options="swiperOption">
      <swiper-slide v-for="item in swiperList" :key="item.id">
        <img class="swiper_img" :src="item.imgUrl" alt="">
      </swiper-slide>
      <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default {
  name: 'HomeSwiper',
  data: function () {
    return {
      swiperOption: {
        pagination: {
          el: '.swiper-pagination'
        },
        loop: true
      },
      swiperList: [{
        id: '1001',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1809/ff/1bf7d3a4f6591002.jpg_750x200_40809f2a.jpg'
      }, {
        id: '1002',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1810/e0/c99056cd01148902.jpg_750x200_8b93d0b5.jpg'
      }, {
        id: '1003',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1810/c6/0ad5c6d880b45002.jpg_750x200_bbe70a7d.jpg'
      }]
    }
  }
}
</script>

<style scoped>
.swiper_img{
  width: 100%;
}
.wrapper >>> .swiper-pagination-bullet-active{
  background: #fff !important;
}
</style>
