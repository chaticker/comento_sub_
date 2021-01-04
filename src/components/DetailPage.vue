<template>
    <div class="detail">
        <div id="content">
            <div>
                <h3 id="title">Title Title Title Title Title Title Title Title Title Title Title Title Title Title Title Title Title Title Title Title Title Title Title Title T
itle Title Title Title Title Title Title Title Title Title Title Title Title Title</h3>
                <p class="contents">contents contents contents contents contents contents contents contents contents contents contents contents contents contents contents conte
nts contents contents contents contents contents contents contents contents contents contents contents contents contents contents contents co
ntents contents contents contents contents contents contents contents contents contents contents</p>
                <p class="created_atYYYY-MM-dd">create_at(YYYY-MM-dd)</p>
            </div>
        </div>
        
        <p id="answer">답변</p>
        <p id="answer_num">2</p>

        <div id="content2">
            <div>
                <p id="reply_user_name ">reply_user_name</p>
                <hr>
                <p class="contents">contents contents contents contents contents contents contents contents contents contents contents contents contents contents contents conte
nts contents contents contents contents contents contents contents contents contents contents contents contents contents contents contents co
ntents contents contents contents contents contents contents contents contents contents contents</p>
                <p class="created_atYYYY-MM-dd">create_at(YYYY-MM-dd)</p>
            </div>
        </div>

        <div id="content3">
            <div>
                <p id="reply_user_name ">reply_user_name</p>
                <hr>
                <p class="contents">contents contents contents contents contents contents contents contents contents contents contents contents contents contents contents conte
nts contents contents contents contents contents contents contents contents contents contents contents contents contents contents contents co
ntents contents contents contents contents contents contents contents contents contents contents</p>
                <p class="created_atYYYY-MM-dd">create_at(YYYY-MM-dd)</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: "DetailPage",
  props: {
    msg: String,
  },
};
</script>

<style scoped>
#content{
    width: 1140px;
    height: 211px;
    margin: 50px 390px 30px;
    padding: 20px 93px 20px 30px;
    border-radius: 5px;
    -webkit-backdrop-filter: blur(30px);
    backdrop-filter: blur(30px);
    border: solid 1px #00c854;
    background-color: #ffffff;
}

p{
    display: inline-block;
    font-family: SpoqaHanSans;
    font-size: 13px;
    font-weight: normal;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.92;
    letter-spacing: normal;
    color: #7e848a;
}
#title{
    width: 1011px;
    height: 46px;
    margin: 8px 6px 7px 0;
    font-family: SpoqaHanSans;
    font-size: 18px;
    font-weight: bold;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.56;
    letter-spacing: normal;
    text-align: left;
    color: #282c30;
}
.contents{
    width: 1017px;
    height: 66px;
    margin: 13px 0 16px;
    font-family: SpoqaHanSans;
    font-size: 16px;
    font-weight: normal;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.56;
    letter-spacing: normal;
    text-align: left;
    color: #495057;
}

#answer{
    display: inline;
    margin: 0 10px 0 395px;
    color: #00c854;
}
#answer_num{
    margin:0;
}

#content2{
    width: 1205px;
    height: 201px;
    margin: 10px 390px 30px;
    padding: 20px 30px;
    border-radius: 5px;
    -webkit-backdrop-filter: blur(30px);
    backdrop-filter: blur(30px);
    border: solid 1px #e1e4e7;
    background-color: #ffffff;
}
#content3{
    width: 1205px;
    height: 201px;
    margin: 30px 390px 0;
    padding: 20px 30px;
    border-radius: 5px;
    -webkit-backdrop-filter: blur(30px);
    backdrop-filter: blur(30px);
    border: solid 1px #e1e4e7;
    background-color: #ffffff;
}

#reply_user_name{
    width: 124px;
    height: 16px;
    margin: 8px 956px 11px 0;
    font-family: SpoqaHanSans;
    font-size: 16px;
    font-weight: normal;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.56;
    letter-spacing: normal;
    text-align: left;
    color: #7e848a;
}

.created_atYYYY-MM-dd{
    width: 148px;
    height: 13px;
    margin: 20px 869px 2px 0;
    font-family: SpoqaHanSans;
    font-size: 13px;
    font-weight: normal;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.92;
    letter-spacing: normal;
    text-align: left;
    color: #adb5bd;
}
hr{
    width: 1190px;
    height: 0.5px;
    margin: 0 0 5px;
    background-color: #e1e4e7;
}
</style>