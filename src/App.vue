<template>
  <div id="app">
    <nav id="nav_var">
        <p>[01/05] 차성은</p>
    </nav>
    <div id="nav">
      <!-- <router-link to="/">Home</router-link> -->
      <!-- <router-link to="/about">About</router-link> -->
    </div>
    <router-view/>
  </div>
</template>

<script>

</script>

<style lang="scss">
#app{
  width: 1920px;
  height: 827px;
  padding: 0 0 208px;
  background-color: #ffffff;
}
#nav_var{
  width: 1920px;
  height: 70px;
  margin: 0 0 50px;
  padding: 28px 1325px 23px 390px;
  box-shadow: 0 1px 5px 0 rgba(0, 0, 0, 0.07);
  background-color: #ffffff;
}
</style>
