<template>
  <div class="search">
    <input type="text" class="search-input" placeholder="输入城市名或拼音" />
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "CitySearch"
};
</script>

<style lang="less" scoped>
.search {
  height: 0.72rem;
  padding: 0.1rem;
  background-color: #00bcd4;
  .search-input {
    width: 100%;
    box-sizing: border-box;
    padding: 0 0.1rem;
    height: 0.62rem;
    line-height: 0.62rem;
    text-align: center;
    border-radius: 0.06rem;
    color: #666;
  }
}
</style>
