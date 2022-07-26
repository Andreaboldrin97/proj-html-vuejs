<template>
    <div class="container">
        <div class="testimony-text py-5 text-center">
              Why People Talk About
              <span class="brand-name">MaxCoach</span>
              ?
        </div>
        <profileTestimony/>
    </div>
</template>

<script>
import profileTestimony from './profileTestimony.vue' 
export default {
      components :{
         profileTestimony
    },
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.testimony-text{
    font-size: 45px;
    font-weight: 600;
    .brand-name{
        color: $colorBreand;
        font-weight: 200;
    }
}
</style>
