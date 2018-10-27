<template>
    <div>
      <el-row >
        <el-col :span="4" class="menu-bar">兵丰远达</el-col>
        <el-col :span="12" >
          <el-menu
            :default-active="activeIndex"
            class="el-menu-demo"
            mode="horizontal"
            @select="handleSelect"
            background-color="#545c64"
            text-color="#fff"
            active-text-color="#ffd04b">
            <el-menu-item index="1">首页</el-menu-item>
            <el-menu-item index="2">我要买车</el-menu-item>
            <el-menu-item index="3">服务保障</el-menu-item>
            <el-menu-item index="4">联系我们</el-menu-item>
          </el-menu>
        </el-col>
        <el-col :span="8" class="menu-bar">全国服务热线 <i class="el-icon-phone"></i> 400-800-8888</el-col>
      </el-row>
    </div>
</template>

<script>
export default {
  name: 'HomeMenuBar',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      activeIndex: '1'
    }
  },
  methods: {
    handleSelect (key, keyPath) {
      console.log(key, keyPath)
    }
  }
}
</script>

<style scoped>
.menu-bar{
  background-color: #545C64;
  height: 60px;
  color: #FFFFFF;
  line-height: 3.5rem;
}
</style>
