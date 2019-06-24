<template>
  <div id="app">
    <!--布局-->
    <div class="layout">
      <div class="header">
        <!--header的菜单-->
        <mainPage_list_head></mainPage_list_head>
      </div>
      <div class="content">
        <div class="aside">
          <mainPage_list_sider></mainPage_list_sider>
          <div class="list_sider_nav">
          </div>
        </div>
        <div class="main">
          <main_content></main_content>
        </div>
      </div>
      <div class="footer">
        <mainPage_footer></mainPage_footer>
      </div>
    </div>
    <div class="scrollbar-wrap">
      <span class="upbar">
        <a href="/"></a>
      </span>
      <hr id="upbar-line">
      <span class="upinfo">
        回到顶部
      </span>
    </div>
  </div>
</template>

<script>

  import mainPage_list_head from "./components/首页/mainPage_list_head"
  import mainPage_list_sider from "./components/首页/mainPage_list_sider"
  import mainPage_footer from "./components/首页/mainPage_footer"
  import main_content from "./components/内容/main_content"

  export default {
    name: 'mainPage',
    components: {
      mainPage_list_head,
      mainPage_list_sider,
      mainPage_footer,
      main_content,
    }
  }
</script>

<style scoped>
  * {
    margin: 0;
  }

  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    width: 100%;
    background: url("assets/夏目2.jpg") no-repeat fixed;
  }

  .scrollbar-wrap {
    display: block;
    /*height: 60px;*/
    width: 80px;
    right: 200px;
    bottom: 30px;
    text-align: center;
    background: rgba(200, 150, 10, 0.6);
    box-shadow: 5px 5px 6px rgba(40, 40, 10, 0.7);
    font-size: 15px;
    color: #1989fa;
    position: fixed;
    z-index: 110;
  }

  .scrollbar-wrap > .upbar {
    display: block;
    height: 50px;
    width: 30px;
    margin: 5px auto;
    background: url("./assets/返回顶部.png");
    background-size: 95% 100%;
    -moz-transition: background1s;
    -webkit-transition: background1s;
    -o-transition: background1s;
  }

  .scrollbar-wrap > .upinfo {
    display: block;
    box-sizing: border-box;
    height: 22px;
    font-weight: 500;
    margin: 10px 0 5px 0;
    color: wheat;
  }

  #upbar-line {
    margin: 0;
    border: 0;
    height: 2px;
    width: 100%;
    background-color: white;
  }

  .layout {
    height: 1180px;
    width: 1250px;
    margin: 0 auto;
    opacity: 0.85;
    z-index: 1;
  }

  .header {
    width: 100%;
    height: 60px;
    background: forestgreen;
    box-sizing: border-box;
  }

  .content {
    width: 100%;
    height: 1060px;
    background: navajowhite;
    text-align: center;
  }

  .aside {
    width: 20%;
    background: rgb(140, 197, 255);
    display: inline-block;
    float: left;
    height: 100%;
  }

  .main {
    width: 80%;
    height: 100%;
    background: #C0C4CC;
    display: inline-block;
  }

  .footer {
    height: 60px;
    width: 1250px;
    background: forestgreen;
  }


</style>
