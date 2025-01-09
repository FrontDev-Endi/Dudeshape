<template>
  <div class="left animate__animated animate__fadeInLeft">
    <h1 class="title">
      Get Your Best Cosmetic <br />
      Products Here
    </h1>
    <p class="text">
      Lorem Ipsum is simply dummy text of the printing and <br />
      typesetting industry. Lorem Ipsum has been the industry's <br />
      standard dummy
    </p>
    <div class="input">
      <input placeholder="Search" type="search" name="search" id="search" />
      <button type="submit">
        <img src="/public/img/search.svg" alt="search" />
      </button>
    </div>
    <button class="btn">Shop Now</button>
  </div>
</template>

<style scoped>
.left {
  margin-top: 40px;
  .title {
    font-weight: 500;
    font-size: 56px;
    font-size: calc(var(--index) * 2);
    line-height: calc(var(--index) * 2.5);
    color: var(--black);
  }
  .text {
    font-weight: 400;
    font-size: 20px;
    font-size: calc(var(--index) * 0.7);
    margin-top: 30px;
    line-height: 32px;
    line-height: calc(var(--index) * 1);
    color: #555;
  }
  .input {
    margin-top: 30px;
    #search {
      width: calc(var(--index) * 12);
      height: 48px;
      background: var(--white);
      font-weight: 400;
      font-size: 14px;
      line-height: 20px;
      text-transform: capitalize;
      padding-left: 16px;
      padding-right: 60px;
      color: #999;
    }
    button {
      width: 32px;
      height: 32px;
      background: var(--brown);
      z-index: 100;
      margin-left: -48px;
      img {
        margin-top: 3px;
      }
    }
  }
  .btn {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: row;
    margin-top: 60px;
    gap: 10px;
    width: calc(var(--index) * 5.4);
    height: calc(var(--index) * 2);
    background: var(--brown);
    font-weight: 500;
    font-size: 18px;
    font-size: calc(var(--index) * 0.65);
    line-height: 24px;
    color: #fff;
  }
}
</style>
