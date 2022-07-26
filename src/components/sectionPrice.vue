<template>
  <div class="container py-5">
      <div class="text-center">
          <div class="text-focus pb-3">
              CHOOSE A COURSE TO GET STARTED
          </div>
          <div class="service-clients pb-3">
              Latest Featured <span class="service-text">Course</span>
          </div>
      </div>
      <courseCard/>
  </div>
</template>

<script>
import courseCard from './courseCard.vue' 
export default {
          components :{
         courseCard,
      
    },
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
.text-focus{
    font-weight: 200;
}
.service-clients{
    font-size: 40px;
    .service-text{
        color: $colorBreand;
        font-weight: 200;
    }
}

</style>