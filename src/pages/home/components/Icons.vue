<template>
  <div class="icons">
    <div class="icon" v-for="item in iconList" :key="item.id">
      <div class="icon_img">
        <img class="icon_img_style" :src="item.imgUrl" alt="">
      </div>
      <p class="icon_desc">{{item.desc}}</p>
    </div>  
  </div>
</template>

<script>
export default{
  name: 'HomeIcons',
  data: function () {
    return {
      iconList: [{
        id: '1001',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
        desc: '景点门票'
      },{
        id: '1002',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
        desc: '景点门票'
      },{
        id: '1003',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
        desc: '景点门票'
      },{
        id: '1004',
        imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
        desc: '景点门票'
      }]
    }
  }
}
</script>

<style scoped>
.icons{
  width: 100%;
  height: 0;
  padding-bottom: 50%;
  background: green;
  overflow: hidden;
}
.icon{
  width: 25%;
  height: 0;
  padding-bottom: 25%;
  float: left;
  /* background: red; */
  position: relative;
}
.icon_img{
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: .44rem;
}
.icon_img_style{
  height: 100%;
  display: block;
  margin: 0 auto;
}
.icon_desc{
  position: absolute;
  left: 0;
  right: 0;
  bottom: 0;
  height: .44rem;
  line-height: .44rem;
  text-align: center;
}
</style>
