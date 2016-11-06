<template>
  <div id="app">
    <el-row>
      <el-col :span="6">
        <Left />
      </el-col>
      <el-col :span="12">
        <Middle />
      </el-col>
      <el-col :span="6">
        
      </el-col>
    </el-row>
  </div>
</template>

<script>
import Left from './components/Left'

export default {
  name: 'app',
  components: {
    Left
  }
}
</script>

<style scoped>
#app {
  padding: 50px;
  text-align: center;
}

div {
  border: solid red 1px;
}
</style>