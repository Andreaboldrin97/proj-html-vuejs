<template>
  <div class="card-form p-4">
      <i class="py-3" :class="icon"></i>
     <div class="card-text">
         <div class="title-card">
             {{ title }}
         </div>
         <div class="card-content pt-3">
             {{ content }}
         </div>
     </div>
  </div>
</template>

<script>
export default {
    props : {
        icon : String,
        title : String,
        content : String
    }
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