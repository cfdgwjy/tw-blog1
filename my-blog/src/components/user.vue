<template>
  <div class="main">
    <div>
      <el-image
          class="img"
          :src="url"
      >
      </el-image>
    </div>
    <div style="margin-top: 20px">
      <span class="username">tianhaoran</span>
    </div>
    <div class="userinfo" style="margin-top: 20px">
      <div>
       <a>
        <span>{{blog}}</span>
        <span>日志</span>
       </a>
      </div>
      <div>
        <a>
          <span>{{category}}</span>
          <span>分类</span>
        </a>
      </div>
      <div>
        <a>
          <span>{{tag}}</span>
          <span>标签</span>
        </a>
      </div>
      </div>

  </div>
</template>

<script>
import jpg from "../assets/logo.jpg"

export default {
  name: "user",
  data() {
    return {
      url: jpg,
      blog:42,
      category:10,
      tag:6
    }
  }
}
</script>

<style lang="scss" scoped>
.main {

  position: absolute;
  left: 5%;
  width: 15%;

  .username {
    margin: 10px 0 0;
    text-align: center;
    color: cornflowerblue;
    font-weight: normal;
  }
.userinfo{
  div{
    display: inline;
    a{
      display: inline-grid;
      padding-right: 10px;
    }

  }
}
  .img {
    //img{
    width: 100px;
    height: 100px;
    //}

    border: 1px solid grey;
  }
}

</style>