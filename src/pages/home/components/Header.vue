<template>
  <div class="header">
    <div class="header_left">
      <div class="iconfont">&#xe6bc;</div>
    </div>
    <div class="header_input">
      <span class="iconfont">&#xe662;</span>
      热门景点游玩主题
    </div>
    <div class="header_right">
      成都
      <span class="iconfont">&#xe6aa;</span>
    </div>
  </div>
</template>

<script>
export default{
  name: 'HomeHeader'
}
</script>

<style scoped>
.header{
  height: .88rem;
  line-height: .88rem;
  background: #00bcd4;
  display: flex;
  color: #fff;
}
.header_left{
  float: left;
  width: .60rem;
}
.header_input{
  flex: 1;
  background: #fff;
  border-radius: 3px;
  height: .64rem;
  line-height: .64rem;
  margin-top: .12rem;
  color: #333;
}
.header_right{
  float: right;
  width: 1.3rem;
  text-align: center;
}
</style>
