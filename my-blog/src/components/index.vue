<template>
  <div>
    <el-container>
      <el-header>
        <Header></Header>
      </el-header>
      <el-container>
        <el-aside width="200px">
          <User></User>

        </el-aside>
        <el-main>
          <Content1></Content1>
        </el-main>
      </el-container>


    </el-container>


  </div>
</template>

<script>

import Header from "@/components/header";
import Content1 from "@/components/content";
import User from "@/components/user";

export default {
  name: "index",
  components: {User, Content1, Header}
}
</script>

<style scoped>

</style>