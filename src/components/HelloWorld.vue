<template>
  <div class="hello">
    <el-container class="container">
      <el-header class="header">
        <span>老子明天要上班，一点也不爽！</span>
      </el-header>
      <el-container>
        <el-aside class="aside"></el-aside>
        <el-main class="main"></el-main>
      </el-container>
    </el-container>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: ["msg"]
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello {
  height: 100%;
}
.aside {
  background-color: rgb(15, 218, 32);
}
.main {
  background-color: #e9e9e9;
}
.container{
  height: 100%;
}

</style>
