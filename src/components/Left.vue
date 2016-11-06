<template>
  <div class="left">
    <div class="top">
      <span></span>
      <p>小二狗</p>
    </div>
    <div class="bottom">
      <p>技术栈</p>
      <div>
        <span class="col1">Vue 2.0</span>
        <span class="col2">vue-resource</span>
        <span class="col3">element-ui</span>
        <span class="col4">webpack</span>
        <span class="col1">图灵机器人API</span>
        <div style="clear: both;"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'left'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.left {
  margin: 5px;
  border: #dbdada solid 1px;
  box-shadow: #666 0px 0px 5px;
}
.top {
  padding-top: 40px;
  background: #00a3f0;
}

.top span {
  background: url(/static/images/robot_head.jpg) no-repeat;
  height: 100px;
  width: 100px;
  border-radius: 100px;
  display: block;
  margin: 0 auto;
}

.top p {
  color: #fff;
  line-height: 62px;
}

.bottom p {
  text-align: left;
  padding-left: 30px
}

.bottom div {
  padding-left: 25px;
}
 
.bottom span {
  float: left;
  margin-right: 10px;
  margin-bottom: 16px;
  padding: 5px 12px;
  font-size: 14px;
  border-radius: 4px;
}

.col1 {
  color: #3cb1e7;
  border: #3cb1e7 solid 1px;
}

.col2 {
  color: #ff9c01;
  border: #ff9c01 solid 1px;
}

.col3 {
  color: #009944;
  border: #009944 solid 1px;
}

.col4 {
  color: #6e61a9;
  border: #6e61a9 solid 1px;
}
</style>
