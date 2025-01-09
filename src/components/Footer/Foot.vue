<template>
  <div class="foot">
    <div class="one">
      <h1 class="logo">Dudeshape</h1>
      <p class="text">
        Lorem Ipsum is simply dummy text of the printing and typesetting
        industry. Lorem Ipsum has been the industry's standard dummy
      </p>
    </div>
    <div class="bloc">
      <div class="two">
        <h1 class="title">Quick Link</h1>
        <ul>
          <li>Home</li>
          <li>Products</li>
          <li>About Us</li>
        </ul>
      </div>
      <div class="three">
        <h1 class="title">Contact Us</h1>
        <p>oyasimnaeem@email.com</p>
        <p>+123456789</p>
        <div class="icon">
          <img src="/img/facebook 1.png" alt="facebook" />
          <img src="/img/instagram 1.png" alt="instagram" />
          <img src="/img/twitter 1.png" alt="twitter" />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.foot {
  margin-top: 60px;
  padding-bottom: 52px;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  margin-left: auto;
  margin-right: auto;
  .one {
    margin-right: calc(var(--index) * 7.4);
    .logo {
      font-style: italic;
      font-weight: 700;
      font-size: calc(var(--index) * 1.5);
      line-height: calc(var(--index) * 1.8);
      text-decoration: underline;
      text-decoration-skip-ink: none;
      color: #222;
    }
    .text {
      margin-top: 38px;
      font-weight: 400;
      font-size: 18px;
      font-size: calc(var(--index) * 0.6);
      width: calc(var(--index) * 12);
      line-height: calc(var(--index) * 1.2);
      color: #555;
    }
  }
  .bloc {
    display: flex;
    /* flex-direction: column; */
    .two {
      margin-top: 25px;
      /* margin-left: 212px; */
      .title {
        font-weight: 500;
        font-size: calc(var(--index) * 0.7);
        line-height: calc(var(--index) * 1);
        color: #222;
      }
      ul {
        /* margin-top: 40px; */
        margin-top: calc(var(--index) * 1);
        li {
          font-weight: 400;
          cursor: pointer;
          font-size: calc(var(--index) * 0.6);
          line-height: calc(var(--index) * 0.8);
          color: #222;
          padding-bottom: 20px;
        }
      }
    }
    .three {
      margin-top: 25px;
      /* margin-left: 213px; */
      margin-left: calc(var(--index) * 7.5);
      .title {
        font-weight: 500;
        font-size: calc(var(--index) * 0.7);
        line-height: calc(var(--index) * 1);
        color: #222;
        padding-bottom: calc(var(--index) * 1);
      }
      p {
        font-weight: 400;
        cursor: pointer;
        font-size: calc(var(--index) * 0.6);
        line-height: calc(var(--index) * 0.8);
        color: #222;
        padding-bottom: 20px;
      }
      .icon {
        display: flex;
        gap: 30px;
      }
    }
  }
}

@media (max-width: 760px) {
  .foot {
    flex-direction: column;
    .one {
      margin-right: 0px;
      margin-left: auto;
      margin-right: auto;
    }
  }
}
</style>
