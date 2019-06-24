<template>
  <div id="App">
    <div class="mainPage_list_sider">
      <div class="personal">
        <div class="personal-info">
          <div class="personal-info-head">
            <img src="../../assets/square-head.jpeg" title="T_T隨便找的頭像" alt="頭像">
          </div>
          <div class="personal-info-name">Channing<br/>的個人主頁</div>
        </div>
        <div class="personal-info-view">
          <!--{{viewNumber}}-->
          <div class="personal-info-view-num">歷史訪客數量:<span class="view-num">19999</span></div>
          <div class="personal-info-click">點我有驚喜~~~</div>
        </div>
      </div>
      <ul class="items-list">
        <li class="list_sider" id="list_sider1">
          <a href="#">頁面1</a>
        </li>
        <li class="list_sider" id="list_sider2">
          <a href="#">頁面2</a>
        </li>
        <li class="list_sider" id="list_sider3">
          <a href="#">頁面3</a>
        </li>
        <li class="list_sider" id="list_sider4">
          <a href="#">頁面4</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
  export default {
    name: "mainPage_list_sider",
    methods: {
      handleOpen(key, keyPath) {
        console.log(key, keyPath);
      },
      handleClose(key, keyPath) {
        console.log(key, keyPath);
      }
    }
  }
</script>

<style scoped="">
  .mainPage_list_sider {
    margin: 10px auto 50px;
  }

  .personal{
    font-size: 15px;
    font-weight: 600;
    color: #616266;
  }

  .list_sider {
    display: block;
    box-sizing: border-box;
    width: 100%;
    height: 40px;
    line-height: 40px;
    text-align: center;
    vertical-align: middle;
    font-weight: 400;
    font-size: 15px;
    transition: 0.3s ease-in-out;
  }

  .list_sider:hover {
    background: rgb(83, 168, 255);
    font-weight: 600;
    border-right: 2px solid white;
    cursor: pointer;
    transition: 0.3s ease-in-out;
    box-shadow:  2px 0 2px gray;
  }

  ul, li {
    list-style-type: none;
    padding: 0;
    margin: 0
  }

  .mainPage_list_sider ul li a {
    text-decoration: none;
    color: black
  }

  .mainPage_list_sider ul li a:visited {
    color: #909399;
  }

  .mainPage_list_sider>.items-list{
    display: block;
    background: snow;
    border: 1px solid gray;
    border-radius: 10px;
    margin: 7px 7px 5px 5px;
    box-shadow: 4px 5px 3px gray;
  }

  .personal-info {
    background: ghostwhite;
    margin: 5px 7px 0 5px;
    border: 1px solid gray;
    height: 120px;
    border-top-left-radius: 10px;
    border-top-right-radius: 10px;
    box-shadow: 4px 4px 3px gray;
  }

  .personal-info > .personal-info-head {
    border: 1px solid black;
    width: 70px;
    height: 70px;
    margin: 25px auto auto 17px;
    border-radius: 70px;
    display: inline-block;
    float: left;
  }

  .personal-info > .personal-info-head>img{
    height: 70px;
    width: 70px;
    overflow: hidden;
    border-radius: 70px;
  }

  .personal-info > .personal-info-name{
    text-align: center;
    line-height:30px ;
    color: #000000;
    font-weight: 600;
    font-size: 18px;
    font-family:Helvetica, 'Hiragino Sans GB', 'Microsoft Yahei', '微软雅黑', Arial, sans-serif;
    display: inline-block;
    margin:28px auto auto 17px;
    float: left;
  }

  .personal > .personal-info-view {
    background: ghostwhite;
    margin: 0 7px 2px 5px;
    border: 1px solid gray;
    height: 150px;
    border-bottom-left-radius: 10px;
    border-bottom-right-radius: 10px;
    box-shadow: 4px 4px 3px gray;
  }

  .personal > .personal-info-view>.personal-info-view-num{
    margin: 5px 0 auto 0;
    text-align: center;
    line-height: 50px;
  }

  .personal > .personal-info-view>.personal-info-view-num>.view-num{
    color:blue;
  }

  .personal > .personal-info-view>.personal-info-click{
    text-align: center;
    line-height: 50px;
    width: 200px;
    margin: auto;
    border: dashed red 2px ;
  }

  #list_sider1 {

  }

  #list_sider2 {

  }

  #list_sider3 {

  }

  #list_sider4 {

  }
</style>
