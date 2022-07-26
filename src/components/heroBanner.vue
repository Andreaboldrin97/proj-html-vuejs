<template>
  <div class="d-flex justify-content-center position-relative banner-container">
      <div class="d-flex align-items-end">
          <img src="../assets/remote-training/images/home-6-hero-left-person-244x300.png" alt="">
      </div>
      <div class="position-relative border-hero">
            <img src="../assets/remote-training/images/home-6-hero-poster-final.jpg" alt="">
          <div class="position-absolute top-50 start-50 img-play">
               <img src="../assets/remote-training/images/icon-youtube-play.png" alt="">
          </div>
      </div>
      <div class="d-flex align-items-end">
           <img src="../assets/remote-training/images/home-6-hero-right-person-195x300.png" alt="">
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
img{
    width: 100%;
}
.banner-container{
    top: 60px;
}
.border-hero{
    border: 12px solid white;
    border-radius: 10px;
}
.img-play{
    transform: translate(-50% , -50%);
}
</style>