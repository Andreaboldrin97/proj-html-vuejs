<template>
  <div class="container text-white text-center p-5">
      <div class="text-focus">{{ focus }}</div>
      <div class="pt-2 pb-4 text_info">{{ textInfo }}</div>
      <a :href="btnLink" class="btn btn_focus text-white px-4"> {{ btnFocus }}</a>
  </div>
</template>

<script>
export default {
 props :{
     focus : String,
     textInfo: String,
     btnFocus : String,
     btnLink : String
 }
}
</script>

<style lang="scss" scoped>
.text-focus{
    font-size: 45px;
}
.text_info{
    font-size: 13px;
    color: #bcbcbc;
}
.btn_focus{
    background-color: #1fad96;
}

</style>