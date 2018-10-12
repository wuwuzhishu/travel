<template>
  <div class="header">
    <div class="header_left">
      左
    </div>
    <div class="header_input">
      中
    </div>
    <div class="header_right">
      右
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
  background: red;
  display: flex;
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
}
.header_right{
  float: right;
}
</style>


