<template>
  <section>
    <div class="container d-flex justify-content-between align-items-center h-100 w-100">
      <div class="w-25">
        <button>SIGN-UP NOW!</button>
      </div>
      <div class="d-flex w-75 justify-content-end">
        <div class="d-flex">
          <h3 class="me-3">FOLLOW US</h3>
        </div>
        <div class="d-flex justify-content-evenly w-25">
          <img src="../assets/footer-facebook.png" alt="facebook">
          <img src="../assets/footer-twitter.png" alt="facebook">
          <img src="../assets/footer-youtube.png" alt="facebook">
          <img src="../assets/footer-pinterest.png" alt="facebook">
          <img src="../assets/footer-periscope.png" alt="facebook">
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
    name: 'SocialSection'
}
</script>


<style lang="scss" scoped>

  section {
    height: 130px;
    background-color: #303030;
    position: relative;
    z-index: 2;

    button {
      border: 2px solid #0c7cec;
      background-color: transparent;
      color: white;
      padding: 10px
    }

    h3 {
      color:#0c7cec
    }

    img {
      cursor: pointer;
    }
  }

</style>