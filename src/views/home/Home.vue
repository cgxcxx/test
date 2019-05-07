<template>
  <div class="">
    <home-header></home-header>
    <home-swiper></home-swiper>
    <home-icon></home-icon>
    <home-recommend></home-recommend>
    <home-weekend></home-weekend>
  </div>
</template>

<script>
import HomeHeader from "../../components/Header";
import HomeSwiper from "../../components/Swiper";
import HomeIcon from "../../components/Icon";
import HomeRecommend from "../../components/Recommend";
import HomeWeekend from "../../components/Weekend";
import axios from "axios";
export default {
  name: "Home",
  components: {
    HomeHeader,
    HomeSwiper,
    HomeIcon,
    HomeRecommend,
    HomeWeekend
  },
  methods: {
    getHomeInfo() {
      axios.get("/index.json").then(this.getHomeInfoSucc);
    },
    getHomeInfoSucc(res) {
      console.log(res);
    }
  },
  mounted() {
    this.getHomeInfo();
  }
};
</script>

<style></style>
