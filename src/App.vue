<script setup>
import { gsap } from "gsap";
import { ScrollTrigger } from "gsap/ScrollTrigger";
import { ScrollSmoother } from "gsap-trial/ScrollSmoother";
gsap.registerPlugin(ScrollSmoother, ScrollTrigger);
ScrollSmoother.create({
  wrapper: ".wrapper",
  content: ".content",
  smooth: 1.5,
  effects: true,
})
import Header from "./components/Header/Header.vue";
import Brand from "./components/Brand/Brand.vue";
import OurPorularProduct from "./components/Our Porular Product/Our Porular Product.vue";
import Number from "./components/Number/Number.vue";
import Info from "./components/Info/Info.vue";
import Slayder from "./components/Slayder/Slayder.vue";
import Footer from "./components/Footer/Footer.vue";
</script>

<template>
  <div class="wrapper">
    <div class="content">
      <Header />
      <Brand />
      <OurPorularProduct />
      <Number />
      <Info />
      <Slayder />
      <Footer />
    </div>
  </div>
</template>
