<template>
  <div class="nav">
    <img src="../assets/home.svg" width="20px" alt="">
    <img src="../assets/search.svg" width="20px" alt="">
    <img src="../assets/p-add.svg" width="20px" alt="">
    <div style="position: relative"><img src="../assets/heart.svg" width="20px" alt="" style="position: relative"> <span
        class="s"></span></div>



    <img src="../assets/user.svg" width="20px" alt="">
  </div>
</template>

<script>
  export default {
    components: {},
    name: "Nav",
  };
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  @media (max-width: 576px) {
    .nav {
      display: flex;
      justify-content: space-around;
      position: fixed;
      bottom: 0;
      width: 100%;
      padding: 12px 0px;
      border-top-left-radius: 20px;
      border-top-right-radius: 20px;
      background-color: #ffffff;
      z-index: 4;
    }

    .s {
      position: absolute;
      width: 8px;
      height: 8px;
      background-color: #fc045c;
      border-radius: 50px;
      right: -3px;
      top: 0px;
      display: block;
      cursor: pointer;
      animation: pulse 2s infinite;
    }

    @keyframes pulse {
      0% {
        -moz-box-shadow: 0 0 0 0 rgba(253, 33, 110, 0.4);
        box-shadow: 0 0 0 0 rgba(253, 33, 110, 0.4);
      }

      70% {
        -moz-box-shadow: 0 0 0 10px rgba(253, 93, 149, 0);
        box-shadow: 0 0 0 10px rgba(253, 93, 149, 0);
      }

      100% {
        -moz-box-shadow: 0 0 0 0 rgba(253, 174, 202, 0);
        box-shadow: 0 0 0 0 rgba(253, 174, 202, 0);
      }
    }
  }
</style>