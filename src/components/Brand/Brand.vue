<template>
  <div class="brand">
    <img src="/public/img/Airbnb.png" alt="Airbnb" class="animate__animated animate__fadeInDown animate__delay-1s" />
    <img src="/public/img/Hubspot.png" alt="Hubspot" class="animate__animated animate__fadeInDown animate__delay-2s"/>
    <img src="/public/img/Google.png" alt="Google" class="animate__animated animate__fadeInDown animate__delay-3s"/>
    <img src="/public/img/Microsoft.png" alt="Microsoft" class="animate__animated animate__fadeInDown animate__delay-4s"/>
    <img src="/public/img/Walmart.png" alt="Walmart" class="animate__animated animate__fadeInDown animate__delay-5s"/>
    <img src="/public/img/FedEx.png" alt="FedEx" class="animate__animated animate__fadeInDown animate__delay-5s" />
  </div>
</template>

<style scoped>
.brand {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 8%;
  width: 75%;
  flex-wrap: wrap;
  margin-left: auto;
  margin-right: auto;
  margin-top: 62px;
  padding-bottom: 22.5px;
  img{
    padding-bottom: 20px;
  }
  .fedEx{
    animation-duration: 6s;
  }
}
</style>
