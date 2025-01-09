<script setup>
import WOW from "wow.js";
const wow = new WOW({
  boxClass: "wow",
  animateClass: "animated",
  offset: 0,
  live: true,
});
wow.init();
</script>

<template>
  <div class="head">
    <div class="head">
      <h1 class="title animate__animated animate__fadeInLeft wow">
        Subscribe to Get Our Letest News
      </h1>
      <div class="input animate__animated animate__fadeInRight wow">
        <input type="email" name="email" id="email" placeholder="Enter email" />
        <button type="submit">Subscribe</button>
      </div>
    </div>
  </div>
</template>

<style scoped>
.head {
  display: flex;
  justify-content: center;
  align-content: center;
  flex-wrap: wrap;
  .title {
    font-weight: 500;
    font-size: 36px;
    font-size: calc(var(--index) * 1.3);
    line-height: calc(var(--index) * 1.8);
    /* padding-right: 300px; */
    padding-right: calc(var(--index) * 10);
    color: #222;
    padding-bottom: 20px;
  }
  .input {
    display: flex;
    input {
      width: 386px;
      width: calc(var(--index) * 14);
      height: 56px;
      background: var(--white);
      font-weight: 400;
      font-size: 16px;
      line-height: 20px;
      color: #555;
      padding-left: 18px;
      background: var(--white);
    }
    button {
      margin-top: auto;
      margin-bottom: auto;
      margin-left: -116px;
      background: var(--brown);
      font-weight: 500;
      font-size: 14px;
      font-size: calc(var(--index) * 0.5);
      line-height: 20px;
      width: calc(var(--index) * 3.8);
      height: 40px;
      height: calc(var(--index) * 1.5);
      color: var(--white);
    }
  }
}

@media (max-width: 912px) {
  .head {
    flex-direction: column;
    .title {
      padding-right: 0px;
    }
  }
}

@media (max-width: 760px) {
  .head {
    .input {
      input {
        width: calc(var(--index) * 20);
      }
    }
  }
}
</style>
