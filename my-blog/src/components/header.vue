<template>
<div>
  <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect">
    <el-menu-item index="1">首页</el-menu-item>
    <el-menu-item index="2">分类</el-menu-item>

    <el-menu-item index="3" >归档</el-menu-item>
    <el-menu-item index="4"><a href="https://www.ele.me" target="_blank">关于</a></el-menu-item>
  </el-menu>
</div>
</template>

<script>
export default {
  name: "header",
  data() {
    return {
      activeIndex: '1',
      activeIndex2: '1'
    };
  },
  methods: {
    handleSelect(key, keyPath) {
      console.log(key, keyPath);
    }
  }
}
</script>

<style lang="scss" scoped>
div{
  display: table;
  margin: 0 auto;
  width: 50%;
}
</style>