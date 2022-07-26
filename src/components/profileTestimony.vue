<template>
    <div class="d-flex container-testimony position-relative">
            <div class="img-testimony me-4">
                <span class="bg-testimony position-relative"></span> 
                <img class="testimony-profile position-relative" :src="require(`../assets/remote-training/images/testimonial-avata-02.jpg`)" alt="img-testimony">
                <img class="position-relative img-background" src="../assets/remote-training/images/maxcoach-shape-05-150x150.png" alt="">
            </div>
            <div class="align-self-center ps-5">
                <div class="pb-2 review-text">
                    I am free to learn at my pace, follow my owen pace, follow my own schedelu and chose the subject i like. Great study portal for people like me.
                </div>
                <div>
                    <div class="name-tesrimony fs-6 pt-4">
                        MINA HOLLACE 
                    </div>
                    <div class="work-tesrimony pt-2">
                        / Freelancer
                    </div>
                </div>
            </div> 
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";


.bg-testimony{
    display: inline-block;
    width: 100px;
    height: 100px;
    border-radius: 50%;
    background-color: $bgTestimony;
   
}
.img-background{
    left: 40%;
    top: -100%;
}
.img-testimony{
     width: 200px;
    height: 200px;
  .testimony-profile{
      top: -50%;
        z-index: 1;
        object-fit: cover;
        border-radius: 50%;
  }
}
.container-testimony{
    width: 75%;
    margin: 0 auto;
}
.review-text{
    font-size: 30px;
}
.name-tesrimony{
    font-weight: 500;
}
.work-tesrimony{
    font-weight: 200;
    color: $colorTextFocus ;
}

</style>