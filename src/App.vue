<template>
  <div id="app">
    <div class="main-body">
      <leftMenu></leftMenu>
      <right-main></right-main>
    </div>
  </div>
</template>

<script>
  import HelloWorld from "./components/HelloWorld.vue";
  import leftMenu from "./components/index/Menu.vue";
  import rightMain from "./components/index/Main.vue";
  export default {
    name: "App",
    components: {
      leftMenu,
      rightMain
    }
  };
</script>

<style>
  #app {
    font-family: "Helvetica Neue", Helvetica, "PingFang SC", "Hiragino Sans GB", "Microsoft YaHei", "微软雅黑", Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
    height: 100%;
  }
  .main-body{
    height: 100%;
  }
  .el-menu{
    border: none;
  }
</style>
