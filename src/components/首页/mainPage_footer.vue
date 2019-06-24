<template>
  <div class="mainPage_footer">
    <div class="mainPage_footer_left">自由发挥</div>
    <div class="mainPage_footer_right">
      <div class="footer-logo">
        <span class="footer-logo-span footer-logo-github"><img src="../../assets/github.png" alt="github"></span>
        <span class="footer-logo-span  footer-logo-csdn"><img src="../../assets/csdn.png" alt="CSDN"></span>
        <span class="footer-logo-span footer-logo-weibo"><img src="../../assets/微博.png" alt="微博"></span>
        <span class="footer-logo-span footer-logo-qq"><img src="../../assets/QQ.png" alt="QQ"></span>
        <span class="footer-logo-span footer-logo-wechat"><img src="../../assets/微信.png" alt="微信"></span>
      </div>
    </div>
    <div class="mainPage_footer_mid">copyright*******************</div>
  </div>
</template>

<script>
  export default {
    name: "mainPage_footer"
  }
</script>

<style>
  .mainPage_footer {

  }

  .mainPage_footer_left, .mainPage_footer_mid, .mainPage_footer_right {
    display: inline-block;
    height: 60px;
    line-height: 60px;
    font-size: 15px;
    vertical-align: middle;
    box-sizing: border-box;
  }

  .mainPage_footer_left {
    width: 20%;
    background: greenyellow;
    float: left;
  }

  .mainPage_footer_mid {
    background: red;
    width: 50%;
    float: left;
  }

  .mainPage_footer_right {
    width: 30%;
    background: white;
  }

  .mainPage_footer_right > .footer-logo > .footer-logo-span {
    display: inline-block;
    vertical-align: middle;
    width: 40px;
    line-height: 100%;
    margin: auto 8px;
  }

  .mainPage_footer_right > .footer-logo > .footer-logo-span > img {
    width: 40px;
    height: 40px;
  }
</style>
