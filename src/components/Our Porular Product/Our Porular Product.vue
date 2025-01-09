<script setup>
import Item from "./Item.vue";
import { ref } from "vue";

const discover = ref(false);
const see = ref(true);

const addtodiscover = () => {
  discover.value = true;
  see.value = false;
};
</script>

<template>
  <div class="our-porular-product">
    <div class="container">
      <div class="head">
        <div class="text">
          <h1 class="title">Our Porular Product</h1>
          <p class="paragraph">
            Lorem Ipsum is simply dummy text of the printing and typesetting
            industry. <br />
            Lorem Ipsum has been the industry's standard dummy
          </p>
        </div>
        <p class="btn" @click="addtodiscover" v-if="see">
          Discover Our Products
          <img src="/img/Frame-2.svg" />
        </p>
      </div>
      <div class="content">
        <div class="see">
          <Item image="/img/pump-bottle-02 1.png" />
          <Item image="/img/jar-15 1.png" />
        </div>
        <div class="hidden" v-if="discover">
          <Item image="/img/pump-bottle-02 1.png" />
          <Item image="/img/jar-15 1.png" />
          <Item image="/img/pump-bottle-02 1.png" />
          <Item image="/img/jar-15 1.png" />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.our-porular-product {
  margin-top: 130px;
  margin-bottom: 130px;
  .container {
    width: 80%;
    display: flex;
    flex-direction: column;
    margin-left: auto;
    margin-right: auto;
    justify-content: center;
    .head {
      display: flex;
      padding-bottom: 60px;
      .text {
        .title {
          font-weight: 500;
          font-size: calc(var(--index) * 2);
          line-height: calc(var(--index) * 2.5);
          color: var(--black);
        }
        .paragraph {
          font-weight: 400;
          font-size: calc(var(--index) * 0.7);
          margin-top: 20px;
          line-height: calc(var(--index) * 1.2);
          color: #555;
        }
      }
      .btn {
        cursor: pointer;
        margin-left: auto;
        margin-top: 70px;
        margin-top: calc(var(--index) * 2.4);
        font-weight: 500;
        font-size: calc(var(--index) * 0.9);
        line-height: calc(var(--index) * 1.2);
        text-decoration: underline;
        text-decoration-skip-ink: none;
        color: #222;
        transition: all 0.2s ease;
        img {
          margin-left: 8px;
          margin-top: 3px;
        }
      }
      @media (hover: hover) {
        .btn:hover {
          text-decoration: none;
          img {
            transition: all 0.2s ease;
            transform: translateX(6px);
          }
        }
      }
    }
    .content {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      align-items: center;
      gap: calc(var(--index) * 2);
      .see {
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        gap: calc(var(--index) * 2);
      }
      .hidden {
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        gap: calc(var(--index) * 2);
      }
    }
  }
}
</style>
