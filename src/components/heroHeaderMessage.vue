<template>
  <div class="container text-white text-center p-5">
      <div class="text-focus">{{ focus }}</div>
      <div class="pt-2 pb-4 text_info">{{ textInfo }}</div>
      <btnForm
      :btnFocus ="btnFocus"
      :btnLink="btnLink"
      />
  </div>
</template>

<script>
import btnForm from './btnForm.vue' 

export default {
     components :{
        btnForm
    },
 props :{
     focus : String,
     textInfo: String,
     btnFocus : String,
     btnLink : String
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