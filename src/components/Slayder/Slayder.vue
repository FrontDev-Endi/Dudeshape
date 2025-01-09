<script>
import { ref } from "vue";
import Slayd from "./Slayd.vue";
import { Swiper, SwiperSlide } from "swiper/vue";
import { Navigation } from "swiper/modules";
import "swiper/css";
import "swiper/css/navigation";

export default {
  components: {
    Slayd,
    Swiper,
    SwiperSlide,
  },
  setup() {
    const onSwiper = (swiper) => {};
    const onSlideChange = () => {};
    const prev = ref(null);
    const next = ref(null);
    return {
      modules: [Navigation],
      prev,
      next,
      Swiper,
      onSwiper,
      onSlideChange,
    };
  },
};
</script>

<template>
  <div class="slayder">
    <div class="btn">
      <div ref="prev" class="swiper-button-prev"></div>
      <div ref="next" class="swiper-button-next"></div>
    </div>
    <swiper
      class="slayder"
      :navigation="{
        prevEl: prev,
        nextEl: next,
      }"
      :slides-per-view="1"
      :space-between="50"
      @swiper="onSwiper"
      @slideChange="onSlideChange"
      :modules="modules"
    >
      <swiper-slide>
        <Slayd />
      </swiper-slide>
      <swiper-slide>
        <Slayd />
      </swiper-slide>
      <swiper-slide>
        <Slayd />
      </swiper-slide>
      <swiper-slide>
        <Slayd />
      </swiper-slide>
      <swiper-slide>
        <Slayd />
      </swiper-slide>
      <swiper-slide>
        <Slayd />
      </swiper-slide>
    </swiper>
  </div>
</template>

<style scoped>
.slayder {
  width: 80%;
  display: flex;
  padding-bottom: 80px;
  /* justify-content: center;
  align-items: center; */
  margin-left: auto;
  margin-right: auto;
  .btn {
    position: absolute;
    display: flex;
    align-items: center;
    justify-content: center;
    margin-left: 42%;
    margin-top: calc(var(--index) * 17);
    /* margin-top: calc(var(--index) * 15); */
    z-index: 100;
  }
  .swiper-button-next {
    background: url(/img/btn.png) no-repeat;
    background-size: cover;
    width: 32px;
    height: 32px;
    content: none;
    z-index: 100;
    color: transparent;
    left: 0;
    margin-left: 40px;
    /* margin-top: -80px; */
    right: 0;
  }
  .swiper-button-prev {
    background: url(/img/btn.png) no-repeat;
    transform: rotate(180deg);
    background-size: cover;
    width: 32px;
    height: 32px;
    content: none;
    z-index: 100;
    color: transparent;
    left: 0;
    right: 0;
  }
}

@media (max-width: 780px) {
  .slayder {
    padding-bottom: 50px;
  }
}
</style>
