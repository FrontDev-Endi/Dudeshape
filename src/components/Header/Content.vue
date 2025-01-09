<script setup>
  import Left from './Left.vue';
  import Right from './Right.vue';
</script>
<template>
  <div class="content">
    <Left />
    <Right />
  </div>
</template>
<style scoped>
  .content {
    display: flex;
    width: 100%;
    justify-content: center;
    align-items: center;
    margin-right: auto;
    margin-left: auto;
    margin-top: 68px;
    /* z-index: -1;  */
  }
  @media (max-width: 950px) {
    .content {
      flex-direction: column;
    }
  }
</style>