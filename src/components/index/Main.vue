<template>
  <div class="main">Main</div>
</template>
<script>
  export default {
    data() {
      const item = {
        date: '2016-05-02',
        name: '王小虎',
        address: '上海市普陀区金沙江路 1518 弄'
      };
      return {
        tableData: Array(20).fill(item)
      }
    }
  }
</script>
<style scoped>
  .main {
    background-color: #fff;
    height: 100%;
    width: calc(100% - 240px);
    float: right;
  }
  @media (max-width: 768px) {
    .main{
      width: 100%;
      height: auto;
      float: none;
    }
  }
</style>
