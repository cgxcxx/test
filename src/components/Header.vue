<template>
  <div class="header">
    <div class="header-left">
      <i class="iconfont">&#xe624;</i>
    </div>
    <div class="header-input">
      <i class="iconfont">&#xe632;</i>输入城市景点／游玩主题
    </div>
    <router-link to="/city">
      <div class="header-right">
        城市
        <i class="iconfont">&#xe64a;</i>
      </div>
    </router-link>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "HomeHeader",
  components: {}
};
</script>

<style lang="less" scoped>
.header {
  line-height: 0.86rem;
  color: #fff;
  display: flex;
  background-color: #00bcd4;
  .header-left {
    width: 0.64rem;
    text-align: center;
    float: left;
    i {
      font-size: 0.4rem;
    }
  }
  .header-input {
    flex: 1;
    padding-left: 0.2rem;
    height: 0.64rem;
    line-height: 0.64rem;
    margin-top: 0.12rem;
    margin-left: 0.2rem;
    background-color: #fff;
    border-radius: 0.1rem;
    color: #ccc;
  }
  .header-right {
    width: 1.24rem;
    color: #fff;
    text-align: center;
    float: right;
    i {
      font-size: 0.24rem;
    }
  }
}
</style>
