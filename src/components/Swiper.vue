<template>
  <div class="wrap">
    <swiper :options="swiperOption">
      <swiper-slide v-for="item of swiperList">
        <img :src="item.imgUrl" alt="" />
      </swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default {
  name: "HomeSwiper",
  data() {
    return {
      swiperOption: {
        pagination: ".swiper-pagination",
        loop: true
      },
      swiperList: [
        {
          id: "01",
          imgUrl: require("../assets/img/111.png")
        },
        {
          id: "02",
          imgUrl: require("../assets/img/111.png")
        }
      ]
    };
  }
};
</script>
<style lang="less">
.wrap /deep/ .swiper-pagination-bullet-active {
  background: #fff;
}
.wrap {
  width: 100%;
  height: 0;
  overflow: hidden;
  padding-bottom: 50%;
  img {
    width: 100%;
  }
}
</style>
