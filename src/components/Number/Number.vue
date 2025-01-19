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
  <div class="number">
    <div class="content">
      <div class="one animate__animated animate__fadeInDown wow">
        <h1>100%</h1>
        <div class="linea"></div>
        <p>Organic Products</p>
      </div>
      <div
        class="two animate__animated animate__fadeInDown animate__delay-1s wow"
      >
        <h1>2M+</h1>
        <div class="linea"></div>
        <p>Yearly Sales</p>
      </div>
      <div
        class="three animate__animated animate__fadeInDown animate__delay-2s wow"
      >
        <h1>1.9M+</h1>
        <div class="linea"></div>
        <p>Happy Customar</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.number {
  width: 100%;
  margin-bottom: 130px;
  background: var(--pink);
  .content {
    padding-top: 58px;
    padding-bottom: 58px;
    margin-left: auto;
    margin-right: auto;
    width: 75%;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    gap: 23%;
    .one {
      display: flex;
      flex-direction: column;
      align-items: center;
      padding-bottom: 15px;
      h1 {
        font-weight: 700;
        font-size: calc(var(--index) * 2);
        line-height: calc(var(--index) * 2.5);
        color: #222;
      }
      .linea {
        border: 3px solid #222;
        height: 0px;
        width: calc(var(--index) * 5);
      }
      p {
        font-weight: 400;
        font-size: calc(var(--index) * 0.8);
        line-height: calc(var(--index) * 1.2);
        color: #555;
      }
    }
    .two {
      display: flex;
      flex-direction: column;
      align-items: center;
      padding-bottom: 15px;
      h1 {
        font-weight: 700;
        font-size: calc(var(--index) * 2);
        line-height: calc(var(--index) * 2.5);
        color: #222;
      }
      .linea {
        border: 3px solid #222;
        height: 0px;
        width: calc(var(--index) * 5);
      }
      p {
        font-weight: 400;
        font-size: calc(var(--index) * 0.8);
        line-height: calc(var(--index) * 1.2);
        color: #555;
      }
    }
    .three {
      display: flex;
      flex-direction: column;
      align-items: center;
      padding-bottom: 15px;
      h1 {
        font-weight: 700;
        font-size: calc(var(--index) * 2);
        line-height: calc(var(--index) * 2.5);
        color: #222;
      }
      .linea {
        border: 3px solid #222;
        height: 0px;
        width: calc(var(--index) * 5);
      }
      p {
        font-weight: 400;
        font-size: calc(var(--index) * 0.8);
        line-height: calc(var(--index) * 1.2);
        color: #555;
      }
    }
  }
}

@media (max-width: 425px) {
  .number {
    .content {
      .one {
        h1 {
          font-size: calc(var(--index) * 2.5);
          line-height: calc(var(--index) * 2.5);
        }
        .linea {
          width: calc(var(--index) * 5.5);
        }
        p {
          font-size: calc(var(--index) * 0.95);
          line-height: calc(var(--index) * 1.5);
        }
      }
      .two {
        h1 {
          font-size: calc(var(--index) * 2.5);
          line-height: calc(var(--index) * 2.5);
        }
        .linea {
          width: calc(var(--index) * 5.5);
        }
        p {
          font-size: calc(var(--index) * 0.95);
          line-height: calc(var(--index) * 1.5);
        }
      }
      .three {
        h1 {
          font-size: calc(var(--index) * 2.5);
          line-height: calc(var(--index) * 2.5);
        }
        .linea {
          width: calc(var(--index) * 5.5);
        }
        p {
          font-size: calc(var(--index) * 0.95);
          line-height: calc(var(--index) * 1.5);
        }
      }
    }
  }
}

@media (max-width: 320px) {
  .number{
    margin-bottom: calc(var(--index) * 5);
  }
}
</style>
