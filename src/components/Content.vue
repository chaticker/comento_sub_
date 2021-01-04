<template>
  <div class="content">
    <h1>필터</h1>
    <label for="">
        <p><input type="checkbox" checked="checked" id="a"> <label for="a">category_name</label></p>
        <p><input type="checkbox" checked="checked" id="b"> <label for="b">category_name</label></p>
        <p><input type="checkbox" checked="checked" id="c"> <label for="c">category_name</label></p>
    </label>
    <ModalView v-if="isModalViewed" @close-modal="isModalViewed = false">
        <Content/>
    </ModalView>
    <button @click="$emit('close-modal')" id="filter_button">저장하기</button> 
  </div>
</template>

<script>
import ModalView from "@/components/ModalView";
export default {
  name: "Content",
  components: {
    ModalView,
  },
  data() {
    return {
      isModalViewed: false,
    };
  },
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1{
    width: 50px;
    height: 27px;
    margin: 9px 263px 10px 0;
    font-family: SpoqaHanSans;
    font-size: 22px;
    font-weight: bold;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.45;
    letter-spacing: normal;
    text-align: left;
    color: #212529;
}

label{
    font-family: SpoqaHanSans;
    font-size: 16px;
    font-weight: normal;
    font-stretch: normal;
    font-style: normal;
    line-height: 2;
    letter-spacing: normal;
    text-align: left;
    color: #495057;
}

input{
    width: 20px;
    height: 20px;
    margin: 13px 5px 12px 0;
    border: solid 1px #e1e4e7;
    background-color: #ffffff;
}

label[for="a"] {
    position: relative;
    top: -5px;
}

label[for="b"] {
    position: relative;
    top: -5px;
}

label[for="c"] {
    position: relative;
    top: -5px;
}

#filter_button{
    width: 112px;
    height: 40px;
    margin: 40px 3px 0 300px;
    /* padding: 13px 24px 8px 20px; */
    border-radius: 3px;
    background-color: #00c854;
    border: 0;
    outline: 0;
    font-family: SpoqaHanSans;
    font-size: 16px;
    font-weight: normal;
    font-stretch: normal;
    font-style: normal;
    line-height: 2;
    letter-spacing: normal;
    text-align: center;
    color: #ffffff;
    cursor: pointer;
}
p{
    margin: 0;
}
</style>
