<template>
  <div class="header">
    城市选择
    <router-link to="/">
      <div class="header-left">
        <i class="iconfont">&#xe624;</i>
      </div>
    </router-link>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "CityHeader",
  components: {}
};
</script>

<style lang="less" scoped>
.header {
  line-height: 0.86rem;
  color: #fff;
  height: 0.86rem;
  line-height: 0.86rem;
  text-align: center;
  background-color: #00bcd4;
  font-size: 0.32rem;
  position: relative;
  .header-left {
    position: absolute;
    left: 0;
    top: 0;
    width: 0.64rem;
    text-align: center;
    i {
      font-size: 0.4rem;
      color: #fff;
    }
  }
}
</style>
