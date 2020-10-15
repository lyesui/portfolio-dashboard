<template>
  <div class="container">
    <Nuxt />
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
  .container {
    width: 100%;
    height: 100vh;
    min-height: 530px;
    background-image: url('/login_background.jpg');
    background-size: cover;
    background-repeat: no-repeat;

    display: flex;
    align-items: center;
    justify-content: center;
  }
</style>