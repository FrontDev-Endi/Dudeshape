<template>
  <div class="info">
    <div class="content">
      <div class="left">
        <h1 class="title">
          The Perfect Beauty <br />
          Of You
        </h1>
        <div class="paragraph">
          <p>
            Lorem Ipsum is simply dummy text of the printing and typesetting
            <br />
            industry. Lorem Ipsum has been the industry's standard dummy text
            <br />
            ever since the 1500s, when an unknown printer took a galley of type
            <br />
            and scrambled it to make a type specimen book.
          </p>
          <p>
            It has survived not only five centuries, but also the leap into
            electronic <br />
            typesetting, remaining essentially unchanged. Lorem Ipsum is simply
            <br />
            dummy text of the printing and typesetting industry.
          </p>
        </div>
        <button class="btn">Shop Now</button>
      </div>
      <div class="right">
        <img src="./img/Rectangle 8.png" alt="Group 1" />
      </div>
    </div>
  </div>
</template>

<style scoped>
.info {
  width: 100%;
  margin-right: auto;
  margin-left: auto;
  margin-bottom: 130px;
  .content {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    .left {
      padding-bottom: 20px;
      .title {
        font-weight: 500;
        font-size: calc(var(--index) * 2);
        line-height: calc(var(--index) * 2.5);
        color: var(--black);
      }
      .paragraph {
        p {
          font-weight: 400;
          font-size: calc(var(--index) * 0.7);
          line-height: calc(var(--index) * 1.1);
          color: #555;
          margin-top: calc(var(--index) * 0.6);
        }
      }
      .btn {
        cursor: pointer;
        display: flex;
        align-items: flex-start;
        justify-content: flex-start;
        flex-direction: row;
        gap: 10px;
        margin-top: 50px;
        /* padding: 16px 32px; */
        padding: calc(var(--index) * 0.5) calc(var(--index) * 1.2);
        width: calc(var(--index) * 5);
        height: calc(var(--index) * 2);
        background: var(--brown);
        font-weight: 500;
        font-size: calc(var(--index) * 0.56);
        line-height: calc(var(--index) * 0.85);
        color: var(--white);
      }
    }
    .right {
      margin-left: 32px;
      img {
        width: 100%;
        width: calc(var(--index) * 20);
      }
    }
  }
}

@media (max-width: 780px) {
  .info {
    .content {
      .right{
        display: none;
      }
    }
  }
}
</style>
