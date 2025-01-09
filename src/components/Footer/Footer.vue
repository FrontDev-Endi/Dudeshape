<script setup>
  import Head from './Head.vue';
  import Foot from './Foot.vue';
</script>

<template>
  <footer class="footer">
    <div class="container">
      <Head />
      <hr />
      <Foot />
    </div>
  </footer>
</template>

<style scoped>
.footer {
  background: #fafafa;
  .container {
    padding-top: 73px;
    width: 80%;
    display: flex;
    margin-left: auto;
    margin-right: auto;
    flex-direction: column;
    hr {
      border: 1px solid #ddd;
      width: 90%;
      margin-top: 60px;
      height: 0px;
      margin-left: auto;
      margin-right: auto;
    }
  }
}
</style>
