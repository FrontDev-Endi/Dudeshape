<script setup>
  import Menu from './Menu.vue';
  import Content from './Content.vue';
</script>

<template>
  <header class="header">
    <div class="container">
      <Menu />
      <Content />
    </div>
  </header>
</template>

<style scoped>
  .header{
    background: var(--pink);
    .container{
      width: 80%;
      padding-bottom: 80px;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      margin-left: auto;
      margin-right: auto;
    }
  }
</style>