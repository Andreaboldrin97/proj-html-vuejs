<template>
  <div class="container d-flex  position-relative banner-container ">
      <div class="d-flex align-items-end position-relative hero-left">
          <img src="../assets/remote-training/images/home-6-hero-left-person.png" alt="">
      </div>
      <div class="position-relative hero-center mb-4">
            <img src="../assets/remote-training/images/home-6-hero-poster-final.jpg" alt="">
            <div class="position-absolute top-50 start-50 img-play">
                <img src="../assets/remote-training/images/icon-youtube-play.png" alt="">
            </div>
      </div>
      <div class="d-flex align-items-end position-relative hero-right">
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
    right: 5%;
    top: 70px;
    overflow: hidden;
}
.hero-left{
    left: 40px;
}
.hero-center{
    border: 12px solid white;
    border-radius: 10px;
    box-shadow: rgba(0, 0, 0, 0.1) 0px 10px 15px -3px, rgba(0, 0, 0, 0.05) 0px 4px 6px -2px;
    img{
        object-fit: cover;
        object-position: top;
    }
        .img-play{
            transform: translate(-50% , -50%);
        }
}
.hero-right{
    top: 130px;
}

</style>