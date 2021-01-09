<template>
<div class="article">
<div style="left:25%;">
  <span style="font-weight: bold;">Vue3 插件开发详解尝鲜版</span>
  <div style="margin-top: 15px;font-size: 10px; color: #409EFF;">
     <span>发表于
    <span>{{date}}</span>
  </span>
    <el-divider direction="vertical"></el-divider>
    <span>分类于
    <span>{{date}}</span>
  </span>
    <el-divider direction="vertical"></el-divider>
    <span>阅读数
    <span>{{count}}</span>
  </span>
    <el-divider direction="vertical"></el-divider>
    <span>喜欢数
    <span>{{count}}</span>
  </span>
  </div>
<div class="content">
  <el-button type="success" size="mini" round>阅读全文</el-button>
</div>
</div>
</div>
</template>

<script>
export default {
  name: "content",
  data() {
    return {
      date:'2020-05-28',
      count:11
    };
  },
}
</script>

<style lang="scss" scoped>
.article{
  text-align: left;
  left: 25%;
  position: absolute;
  padding-left: 20px;

  .content{
    margin-top: 20px;
  }
}

</style>