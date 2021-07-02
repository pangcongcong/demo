<template>
  <swiper
    :indicator-dots="bannerIndicatorDots"
    :current="bannerIndex"
    :autoplay="true"
    interval="5000"
    duration="700"
    :circular="true"
    class="banners-swiper"
    indicator-active-color="#969696"
    @change="bannerChange"
  >
    <swiper-item
      v-for="(banner, index) in infoItem"
      class="swiper-item"
      :key="'swiper-item-' + index"
      :id="'swiper-item-' + index"
    >
      <image
        class="banners-image"
        v-if="banner.image"
        :src="
          banner.image 
        "
        mode="widthFix"
        :key="banner.image"
      >
      </image>
    </swiper-item>
  </swiper>
</template>


<script lang="ts">

export default {
  
  data() {
    return {
      bannerIndex: 0,
      infoItem:  [
          {
            "image": "https://j-image.missfresh.cn/img_20210701175140546.png?mryxw=1065&mryxh=360", 
          }, 
          {
            "image": "https://j-image.missfresh.cn/img_20210701184535714.jpg?mryxw=1065&mryxh=360", 
          }, 
          {
            "image": "https://j-image.missfresh.cn/img_20210701184833793.jpeg?mryxw=1065&mryxh=360", 
          }, 
          {
            "image": "https://j-image.missfresh.cn/img_20210701132501740.jpeg?mryxw=1065&mryxh=360", 
          }, 
          {
            "image": "https://j-image.missfresh.cn/img_20210622205132290.jpg?mryxw=1065&mryxh=360", 
          }
      ] 
    };
  },
  computed: {
    
  },
  created() {
    
  },
  detached() {},
  methods: {
    bannerChange(event) {
      
    },

    // 点击banner
    clickBanner(banner,bannerIndex) {
     
    }
  },
};
</script>
