<script setup>
// import { ref, onMounted, onUnmounted } from "vue";
import Header from "./components/Header/Header.vue";
import Brand from "./components/Brand/Brand.vue";
import OurPorularProduct from "./components/Our Porular Product/Our Porular Product.vue";
import Number from "./components/Number/Number.vue";
import Info from "./components/Info/Info.vue";
import Slayder from "./components/Slayder/Slayder.vue";
import Footer from "./components/Footer/Footer.vue";

SmoothScroll({
// Время скролла 400 = 0.4 секунды
animationTime : 800,
// Размер шага в пикселях
stepSize : 75,

// Дополнительные настройки:

// Ускорение
accelerationDelta : 30,
// Максимальное ускорение
accelerationMax : 2,

// Поддержка клавиатуры
keyboardSupport : true,
// Шаг скролла стрелками на клавиатуре в пикселях
arrowScroll : 50,

// Pulse (less tweakable)
// ratio of "tail" to "acceleration"
pulseAlgorithm : true,
pulseScale : 4,
pulseNormalize : 1,

// Поддержка тачпада
touchpadSupport : true,
})
</script>

<template>
  <div id="wrapper">
    <div id="content">
      <Header />
      <Brand />
      <OurPorularProduct />
      <Number />
      <Info />
      <Slayder />
      <Footer />
    </div>
  </div>
  <div id="smooth-scrollbar"></div>
</template>