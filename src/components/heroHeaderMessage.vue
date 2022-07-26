<template>
  <div class="container text-white text-center pt-5">
      <div class="text-focus">{{ focus }}</div>
      <div class="pt-2 pb-4 text_info">{{ textInfo }}</div>
    
  </div>
</template>

<script>


export default {
     
 props :{
     focus : String,
     textInfo: String,
 }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
.text-focus{
    font-size: 45px;
}
.text_info{
    font-size: 13px;
    color: $colorTextFocus;
}


</style>