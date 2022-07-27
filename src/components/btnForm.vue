//! creato components btn
<template>
  <div>
      <a :href="btnLink" class="btn btn_focus text-white px-5 py-2"> {{ btnFocus }}</a>
  </div>
</template>

<script>
export default {

//? props di defaul per il passaggio dei dati

props :{
    btnFocus : String,
    btnLink : String
}
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
.btn_focus{
    background-color: $colorBreand;
}
</style>