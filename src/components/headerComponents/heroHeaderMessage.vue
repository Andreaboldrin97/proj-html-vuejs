<template>
  <div class="container text-white text-center pt-5">
      <div class="text-focus">
          Learn At Own Pace!
      </div>
      <div class="pt-2 pb-4 text_info">
          Get teamed up whith peoople of the same will.
      </div>
    
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
@import "./src/style/variables.scss";
.text-focus{
    font-size: 55px;
    font-weight: 500;
}
.text_info{
    font-size: 18px;
    font-weight: 500;
    color: $colorTextFocus;
}


</style>