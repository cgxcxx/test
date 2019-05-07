<template>
  <div class="icons">
    <swiper>
      <!-- slides -->
      <swiper-slide v-for="(page, index) of pages">
        <div class="icon-item" v-for="item of page">
          <div class="icon-img">
            <img :src="item.imgUrl" alt="" />
          </div>
          <p>{{ item.desc }}</p>
        </div>
      </swiper-slide>
    </swiper>
  </div>
</template>

<script>
export default {
  name: "HomeIcon",
  data() {
    return {
      iconList: [
        {
          id: "0001",
          imgUrl: require("../assets/img/icon.png"),
          desc: "出境游1"
        },
        {
          id: "0002",
          imgUrl: require("../assets/img/icon.png"),
          desc: "出境游2"
        },
        {
          id: "0003",
          imgUrl: require("../assets/img/icon.png"),
          desc: "出境游3"
        },
        {
          id: "0004",
          imgUrl: require("../assets/img/icon.png"),
          desc: "出境游4"
        },
        {
          id: "0005",
          imgUrl: require("../assets/img/icon.png"),
          desc: "出境游5"
        },
        {
          id: "0006",
          imgUrl: require("../assets/img/icon.png"),
          desc: "出境aaaaaaaaaaaaaa游6"
        },
        {
          id: "0007",
          imgUrl: require("../assets/img/icon.png"),
          desc: "出境游7"
        },
        {
          id: "0008",
          imgUrl: require("../assets/img/icon.png"),
          desc: "出境游8"
        },
        {
          id: "0009",
          imgUrl: require("../assets/img/icon.png"),
          desc: "出境游9"
        }
      ]
    };
  },
  computed: {
    pages() {
      const pages = [];
      this.iconList.forEach((item, index) => {
        const page = Math.floor(index / 8);
        if (!pages[page]) {
          pages[page] = [];
        }
        pages[page].push(item);
      });
      return pages;
    }
  }
};
</script>
<style lang="less">
.icons /deep/ .swiper-container {
  height: 0;
  padding-bottom: 50%;
}
.icons {
  .icon-item {
    position: relative;
    float: left;
    width: 25%;
    height: 0;
    padding-bottom: 25%;
    .icon-img {
      position: absolute;
      box-sizing: border-box;
      padding: 0.1rem;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0.44rem;
      img {
        height: 100%;
        display: block;
        margin: 0 auto;
      }
    }
    p {
      position: absolute;
      height: 0.44rem;
      line-height: 0.44rem;
      text-align: center;
      left: 0;
      right: 0;
      bottom: 0;
      overflow: hidden;
      white-space: nowrap;
      text-overflow: ellipsis;
    }
  }
}
</style>
