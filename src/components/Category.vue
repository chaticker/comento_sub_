<template>
    <div class="category">
        <router-link to="/detail">
            <div id="content1">
                <p id="category_name">category_name</p>
                <p id="contents_id">contents_id</p>
                <hr>
                <p id="user_id">user_id</p><p>| create_at(YYYY-MM-dd)</p>
                <h1 id="title">Title</h1>
                <h4 id="contents">contents</h4>
            </div>
        </router-link>

        <router-link to="/detail">
            <div id="content2">
                <p id="sponsored">sponsored</p>
                <img src="" alt="">
                <h1 id="title">Title</h1>
                <h4 id="contents">contents</h4>
            </div>
        </router-link>
        <router-view/>
    </div>
</template>

<script>
export default {
}
</script>

<style scoped>
#content1{
    display: inline-block;
    width: 865px;
    height: 179px;
    margin: 11px 390px 30px 670px;
    padding: 10px 30px 21px;
    border-radius: 5px;
    -webkit-backdrop-filter: blur(30px);
    backdrop-filter: blur(30px);
    border: solid 1px #e1e4e7;
    background-color: #ffffff;
  }

#content2{
    width: 865px;
    height: 255px;
    margin: 30px 390px 0 670px;
    padding: 10px 30px 21px;
    border-radius: 5px;
    -webkit-backdrop-filter: blur(30px);
    backdrop-filter: blur(30px);
    border: solid 1px #e1e4e7;
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
#contents_id{
    float: right;
}

#sponsored{
    width: 61px;
    height: 13px;
    margin: 75px 5px 17px 0;
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
h1{
    margin: 0;
}

hr{
    width:865px;
    height: 0.5px;
    margin: 0 0 5px;
    background-color: #e1e4e7;
}

</style>