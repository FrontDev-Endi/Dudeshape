<script setup>
defineProps({
  image: String,
});
</script>

<template>
  <div class="item">
    <img class="image" :src="image" alt="image" />
    <div class="content">
      <h1 class="title">Cosmetic products</h1>
      <p class="paragraph">
        Lorem Ipsum is simply dummy text of the printing and typesetting
        industry. Lorem Ipsum has been the industry's standard dummy
      </p>
      <div class="bottom">
        <button class="buy">Buy Now</button>
        <button class="add">Add To Cart</button>
        <p class="price">$120</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.item {
  border: 1px solid rgba(104, 90, 82, 0.19);
  width: calc(var(--index) * 20);
  height: calc(var(--index) * 29);
  .content {
    margin-left: calc(var(--index) * 1.2);
    .title {
      margin-top: calc(var(--index) * 0.8);
      font-weight: 500;
      font-size: calc(var(--index) * 1.5);
      line-height: calc(var(--index) * 2.3);
      color: #222;
    }
    .paragraph {
      font-weight: 400;
      font-size: calc(var(--index) * 0.7);
      line-height: calc(var(--index) * 1);
      color: #555;
      /* margin-top: 16px; */
      margin-top: calc(var(--index) * 0.6);
    }
    .bottom {
      display: flex;
      margin-top: 48px;
      .buy {
        display: flex;
        align-items: flex-start;
        justify-content: center;
        align-items: center;
        flex-direction: row;
        gap: 10px;
        width: calc(var(--index) * 5);
        height: calc(var(--index) * 2);
        background: var(--brown);
        font-weight: 500;
        font-size: calc(var(--index) * 0.65);
        line-height: 24px;
        color: var(--white);
        transition: all 0.2s ease;
      }
      @media (hover: hover) {
        .buy:hover {
          background: none;
          border: 1px solid rgba(104, 90, 82, 0.46);
          font-weight: 500;
          font-size: calc(var(--index) * 0.65);
          line-height: 24px;
          color: var(--brown);
        }
      }
      @media (hover: none) {
        .buy:hover {
          background: none;
          border: 1px solid rgba(104, 90, 82, 0.46);
          font-weight: 500;
          font-size: calc(var(--index) * 0.65);
          line-height: 24px;
          color: var(--brown);
        }
      }
      .add {
        display: flex;
        align-items: flex-start;
        justify-content: center;
        align-items: center;
        flex-direction: row;
        gap: 10px;
        width: calc(var(--index) * 5);
        height: calc(var(--index) * 2);
        border: 1px solid rgba(104, 90, 82, 0.46);
        font-weight: 500;
        font-size: calc(var(--index) * 0.65);
        line-height: 24px;
        color: var(--brown);
        margin-left: calc(var(--index) * 0.9);
        transition: all 0.2s ease;
      }
      @media (hover: hover) {
        .add:hover {
          background: var(--brown);
          font-weight: 500;
          font-size: calc(var(--index) * 0.65);
          line-height: 24px;
          color: var(--white);
        }
      }
      @media (hover: none) {
        .add:hover {
          background: var(--brown);
          font-weight: 500;
          font-size: calc(var(--index) * 0.65);
          line-height: 24px;
          color: var(--white);
        }
      }
      .price {
        font-weight: 500;
        font-size: calc(var(--index) * 1.1);
        line-height: calc(var(--index) * 1.4);
        color: #222;
        /* margin-left: 120px; */
        margin-left: calc(var(--index) * 4.3);
        margin-top: 12px;
      }
    }
  }
}

@media (max-width: 425px) {
  .item {
    .content {
      .bottom {
        margin-top: 30px;
      }
    }
  }
}
</style>
