<template>
  <div id="mainContent-App">
    <div class="mainContent-card-bg"
         :style='this.bg.backgroundImage?this.bg:defaultBg'>
    </div>
    <div class="mainContent-card-words">
      <div class="title">
        <p v-html="mainContent_card_title"></p>
      </div>
      <hr>
      <div class="mainContent-card-content">

      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: "mainContent_card_model",
    data() {
      return {
        mainContent_card_title: "然后在div中引用这个类，就可以实现图片透明度设置",
        defaultBg: "",
        bg: {
          backgroundImage: "url(" + require('../../assets/cardbg1.gif') + ")",
          backgroundSize: "auto 100%",
          backgroundRepeat: 'repeat,',
          opacity: '0.3'
        }
      }
    }
  }
</script>

<style scoped>
  #mainContent-App {
    box-sizing: border-box;
    margin: 5px 5px 5px 5px;
    padding: 0;
    height: 200px;
    width: 980px;
    border: solid 1px rgba(0,0,0,0.6);
    border-radius: 10px;
    vertical-align: middle;
    position: relative;
    text-align: left;
  }

  .mainContent-card-bg {
    width: 100%;
    height: 100%;
  }

  .mainContent-card-words {
    width: 100%;
    height: 100%;
    border: none;
    position: absolute;
    z-index: 1;
    /*overflow: hidden;*/
    top: 0;
    vertical-align: middle;
  }

  .mainContent-card-words>.title {
    height: 46px;
    width: 100%;
    margin: 0;
    top: 0;
  }

  .mainContent-card-words>.title > p {
    display: block;
    color: #000;
  }

  .mainContent-card-words>hr {
    margin: 0;
    border: 0;
    height: 2px;
    background: rgba(0, 0, 0, 0.4);
  }

  .mainContent-card-words>.mainContent-card-content {
    height: 150px;
    width: 100%;
  }

</style>
