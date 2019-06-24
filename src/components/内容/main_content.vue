<template>
  <div id="App">
    <div class="mainContent">
      <mainContent_card_model></mainContent_card_model>
      <mainContent_card_model></mainContent_card_model>
      <mainContent_card_model></mainContent_card_model>
      <mainContent_card_model></mainContent_card_model>
      <mainContent_card_model></mainContent_card_model>
    </div>


  </div>
</template>

<script>
  import mainContent_card_model from "./mainContent_card_model"
  export default {
    name:'main_content',
    components:{
      mainContent_card_model,
    }
  }
</script>

<style scoped>
  *{
    margin: 0;
  }

  #App{

  }

  .mainContent{
    box-sizing: border-box;
    margin: 5px 5px 5px 5px;
    padding: 0;
    height: 1050px;
    width: 990px;
    border-radius: 10px;
    border: solid 1px gray;
  }

</style>
