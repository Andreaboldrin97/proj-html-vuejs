<template>
  <div class="card-form">
      <i class="fa-brands fa-font-awesome py-3"></i>
     <div class="card-text">
         <div class="title-card">
             Idea Discussion
         </div>
         <div class="card-content pt-3">
             Get teamed up with the specialists who work and teach coding foe years at famous universities
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

.card-form{
    width: calc(100vw / 4);
    i{
        font-size: 70px;
    }
    .title-card{
        font-weight: 600;
    }
    .card-content{
        font-weight: 300;
        color: $colorTextFocus;
    }
}

</style>