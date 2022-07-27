<template>
  <div class="container banner-content text-center">
      <div class="sub-title">
          Start today for getting <span class="subtitle-focus">Online Certification</span>
      </div>
      <div class="title">
          You can be your own guiding dtar with our help!
      </div>

       <div class="text-center">
          <btnForm class="pt-4"
            :btnFocus ="btnText.btnFocus"
            :btnLink="btnText.btnLink"
            />
      </div>
  </div>
</template>

<script>
import btnForm from './btnForm.vue' 

export default {
        components :{
         btnForm
    },
    data : function(){
        return{
            btnText :{
                    btnFocus : 'Get started now',
                    btnLink : '#'
            }
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.banner-content{
    margin-top: 150px;
}
.sub-title{
    font-size: 20px;
    font-weight: 600;
    .subtitle-focus{
            color: $colorBreand;
            font-weight: 300;
    }
}
.title{
    font-size: 30px;
    font-weight: 600;
}
</style>