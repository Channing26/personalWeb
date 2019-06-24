<template>
  <div id="App">
    <div class="mainPage_list_head">
    <span class="head_list" id="head_list1">
      技术
    </span>
      <span class="head_list" id="head_list2">
      日常
    </span>
      <span class="head_list" id="head_list3">
      音乐
    </span>
      <span class="head_list" id="head_list4">
      链接
    </span>
    </div>
  </div>
</template>

<script>
  export default {
    name: "mainPage_list_head"
  }
</script>

<style scoped>
  #App{
    text-align: center;
  }
  .mainPage_list_head {

  }

  .head_list {
    box-sizing: border-box;
    border: 1px;
    display: inline-block;
    width: 150px;
    height: 60px;
    padding: 0;
    line-height: 60px;
    text-align: center;
    vertical-align: middle;
    color: #ffffff;
    font-weight: 400;
    font-size: 22px;
    transition: 0.3s ease-in-out;
  }

  .head_list:hover {
    background-color: darkgreen;
    font-weight: 600;
    color: yellow;
    border-bottom: 2px solid white;
    cursor: pointer;
    transition: 0.3s ease-in-out;
  }

  #head_list1 {

  }

  #head_list2 {

  }

  #head_list3 {

  }

  #head_list4 {

  }

</style>
