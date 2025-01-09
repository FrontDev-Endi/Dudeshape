<template>
  <div class="slayd">
    <div class="left">
      <img src="/img/pretty.png" alt="pretty" />
    </div>
    <div class="right">
      <div class="content">
        <h1 class="title">Amazing Cosmetic</h1>
        <div class="star">
          <img src="/img/star.png" alt="star" />
        </div>
        <div class="text">
          <p class="paragraph">
            <img class="quote" src="/img/“.svg" />
            Lorem Ipsum is simply dummy text of the printing and typesetting
            industry. Lorem Ipsum has been the industry's standard dummy text
            ever since the 1500s, when an unknown printer took a galley of type
            and scrambled it to make a type specimen book
            <img class="quote-two" src="/img/12.svg" />
          </p>
        </div>
        <h1 class="name">Rusmin Islam</h1>
        <p class="job">Designer</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
  .slayd {
  display: flex;
  justify-content: center;
  .left {
    img {
      width: calc(var(--index) * 20);
      /* width: 100%; */
    }
  }
  .right {
    margin-left: 37px;
    .content {
      .title {
        font-weight: 500;
        font-size: calc(var(--index) * 1.1);
        line-height: calc(var(--index) * 1.5);
        color: #222;
      }
      .star {
        margin-top: 12px;
      }
      .text {
        margin-top: calc(var(--index) * 0.8);
        width: calc(var(--index) * 19);
        .quote {
          margin-left: -17px;
        }
        .paragraph {
          margin-left: 17px;
          font-weight: 400;
          font-size: calc(var(--index) * 0.7);
          line-height: calc(var(--index) * 1.1);
          color: #555;
        }
      }
      .name {
        margin-top: calc(var(--index) * 3);
        font-weight: 500;
        font-size: calc(var(--index) * 1.1);
        line-height: calc(var(--index) * 1.5);
        color: #222;
      }
      .job {
        margin-top: 10px;
        font-weight: 400;
        font-size: calc(var(--index) * 0.7);
        line-height: calc(var(--index) * 1);
        color: #555;
      }
    }
  }
}

@media (max-width: 780px) {
  .slayd {
    .left {
      img {
        display: none;
      }
    }
    .right {
      .content {
        .text {
          margin-top: 10px;
        }
        .name {
          margin-top: 10px;
        }
      }
    }
  }
}
</style>