<template>
  <div id="app">
    <button id="login_button">로그인</button>

    <div id="sort">
      <p class="sort_button">오름차순</p>
      <p class="sort_button">내림차순</p>
      <button @click="isModalViewed = true" id="filter_button">필터</button>
      <ModalView v-if="isModalViewed" @close-modal="isModalViewed = false">
        <Content/>
      </ModalView>  
    </div>

    <div>
      <Category @click="isDetailViewed = true">
        <DetailPage/>
      </Category> 
    </div>
  </div>
</template>

<script>
import ModalView from "@/components/ModalView";
import Content from "@/components/Content";
import Category from "@/components/Category";
import DetailPage from "@/components/DetailPage";
export default {
  name: "MainPage",
  components: {
    ModalView,
    Content,
    Category,
    DetailPage
  },
  data() {
    return {
      isModalViewed: false,
      isDetailViewed: false,
    };
  },
};
</script>

<style scoped>
  #login_button{
    width: 235px;
    height: 60px;
    margin: 50px 40px 0px 390px;
    /* padding: 20px 91px 13px 87px; */
    border-radius: 5px;
    border: 0;
    background-color: #00c854;
    font-family: SpoqaHanSans;
    font-size: 22px;
    font-weight: bold;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.14;
    letter-spacing: normal;
    text-align: center;
    color: #ffffff;
    cursor: pointer;
  }

  #sort{
    display: inline;
    /* position: inherit; */
    /* display: inline; */
    /* margin-left: 700px; */
  }

  .sort_button{
    /* position:inherit; */
    display: inline;
    width: 45px;
    height: 16px;
    margin: 55px 13px 14px 5px;
    font-family: SpoqaHanSans;
    font-size: 13px;
    font-weight: normal;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.92;
    letter-spacing: normal;
    text-align: center;
    color: #495057;
    cursor: pointer;
  }
 
  #filter_button{
    width: 48px;
    height: 24px;
    /* margin: 50px 390px 11px 419px; */
    /* padding: 5px 14px 3px 12px; */
    border-radius: 3px;
    border: solid 1px #e1e4e7;
    background-color: #ffffff;
    cursor: pointer;
    font-family: SpoqaHanSans;
    font-size: 13px;
    font-weight: normal;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.92;
    letter-spacing: normal;
    text-align: center;
    color: #adb5bd;
  }

  #content{
    display: inline-block;
    width: 865px;
    height: 179px;
    margin: 50px 40px 0px 390px;
    padding: 25px 30px 21px;
    border-radius: 5px;
    -webkit-backdrop-filter: blur(30px);
    backdrop-filter: blur(30px);
    border: solid 1px #e1e4e7;
    background-color: #ffffff;
  }
</style>