<template>
  <div class="aside">
    <div class="menu-hide">
      <i v-on:click="toggleMenu" class="menu-hide-btn el-icon-menu"></i>
    </div>
    <menu-list v-bind:class="{hideMenu: isActive}"></menu-list>
  </div>
</template>
<script>
  import MenuList from "./MenuList.vue"
  export default {
    data(){
      return {
        isActive:true,
      }
    },
    components: {
      MenuList,
    },
    methods:{
      toggleMenu: function (event) {
        this.isActive = !this.isActive;
      }
    },
    // mounted () {
    //   const that = this;
    //   window.onresize = () => {
    //     return (() => {
    //       window.screenWidth = document.body.clientWidth;
    //       that.screenWidth = window.screenWidth;
    //     })()
    //   }
    // },
    // watch: {
    //   screenWidth (val) {
    //     this.screenWidth = val;
    //     if(val > 768){
    //       this.willShow = true;
    //     }
    //   }
    // }
  }
</script>
<style scoped>
  .aside {
    background-color: #fff;
    height: 100%;
    border-right: 1px #e6e6e6 solid;
    width: 240px;
    float: left;
  }
  .menu-hide{
    padding: 10px;
    width: 100%;
    overflow: hidden;
    box-sizing: border-box;
    border-bottom: 1px #e6e6e6 solid;
    display: none;
  }
  .menu-hide-btn{
    float: right;
    font-size: 25px;
  }


  @media (max-width: 768px) {
    .aside{
      width: 100%;
      height: auto;
      float: none;
      border-right: none;
    }
    .menu-hide{
      display: block;
    }
    .hideMenu{
      display: none;
    }
  }
</style>
