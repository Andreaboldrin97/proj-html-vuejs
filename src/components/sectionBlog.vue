<template>
  <div class="container py-5">
       <div class="text-center">
          <div class="text-focus pb-3">
              ENJOY READING ON MAXCOACH
          </div>
          <div class="service-blog pb-3">
              Latest On <span class="blog-focus">Our Blogs</span>
          </div>
      </div>
      <blogCard/>
  </div>
</template>

<script>
import blogCard from './blogCard.vue' 

export default {
      components :{
         blogCard
    },
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
.container-card{
    width: 80%;
    margin: 0 auto;
}
.text-focus{
    font-weight: 200;
}
.service-blog{
    font-size: 40px;
    .blog-focus{
        color: $colorBreand;
        font-weight: 200;
    }
}

</style>