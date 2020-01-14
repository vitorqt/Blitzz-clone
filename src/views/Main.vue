<template>
<div class="main">
  <Navbar />

  <div class="container">
    <div class="content">
      <div class="logo">
        <img src="@/assets/img/logo.png" alt="logo">
      </div>
    </div>
  </div>
</div>
</template>

<script>
import Navbar from '@/components/Navbar';

export default {
  name: "main",
  components: {
    Navbar
  }
}
</script>

<style lang="scss">
  .container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 80vh;

    .content {
      height: 500px;
      width: 800px;

      .logo {
        display: flex;
        justify-content: center;
      }
    }
  }



</style>