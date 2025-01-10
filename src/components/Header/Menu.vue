<script setup>
const addtoclass = () => {
  const links = document.querySelector(".links");
  links.classList.toggle("links-active");
};
</script>

<template>
  <div class="menu animate__animated animate__fadeInDown">
    <div class="logo">
      <h1>Dudeshape</h1>
    </div>
    <div class="links">
      <a href="#">Home</a>
      <a href="#">Products</a>
      <a href="#">About Us</a>
      <a href="#">Contact</a>
    </div>
    <div class="ico">
      <img src="./img/Profile.svg" alt="">
      <img class="buy" src="./img/Buy.svg" alt="Buy" />
      <img
        class="frame"
        src="./img/Frame.svg"
        @click="addtoclass()"
        alt="Frame"
      />
    </div>
  </div>
</template>

<style scoped>
.menu {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 95%;
  margin-top: 40px;
  z-index: 100;
  .logo {
    h1 {
      font-style: italic;
      font-weight: 700;
      font-size: 24px;
      line-height: 30px;
      text-decoration: underline;
      text-decoration-skip-ink: none;
      color: #222;
    }
  }
  .links {
    a {
      font-weight: 400;
      font-size: 16px;
      line-height: 20px;
      color: #222;
      text-decoration: none;
      margin-right: 20px;
    }
  }
  .ico {
    display: flex;
    img {
      margin-left: 24px;
    }
    .frame {
      display: none;
    }
  }
}

@media (max-width: 950px) {
  .menu {
    .links {
      position: fixed;
      z-index: 100;
      top: 0;
      transition: 0.5s, visibility 0.5s;
      display: flex;
      flex-direction: column;
      width: 200px;
      height: 88vh;
      margin-left: 88%;
      background: var(--pin);
      right: -200px;
      visibility: hidden; 
      transform: translateX(100%);
      padding-top: 120px;
      align-items: center;
      a {
        margin-right: 0;
        margin-bottom: 20px;
      }
    }
    .links-active {
      visibility: visible;
      transform: translateX(-57%);
      
    }
    .ico {
      .frame {
        position: relative;
        z-index: 101;
        display: block;
      }
    }
  }
}

@media (max-width: 425px) {
  .menu {
    .links {
      right: -156px;
    }
    .links-active {
      visibility: visible;
      transform: translateX(-60%);
    }
  }
}
</style>
