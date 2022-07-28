//! header diviso in 4 components (nav , messaggio centrale , btn components, heroBanner)
<template>
  <header class="hero-header">
    <headerNav/>

    <heroHeaderMessage id="header"/>

      <div class="text-center">
          <btnForm
            btnFocus ="Get started for free"
            btnLink="#"
            onHeader= true
            />
      </div>

    <heroBanner/>

  </header>
</template>

<script>
import headerNav from './headerComponents/headerNav.vue' 
import heroHeaderMessage from './headerComponents/heroHeaderMessage.vue' 
import heroBanner from './headerComponents/heroBanner.vue' 
import btnForm from './btnForm.vue' 

export default {
     components :{
         headerNav,
        heroHeaderMessage,
        heroBanner,
        btnForm
    },
     data : function (){
        return{
           
        }
    }

}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
.hero-header{
    background-color: $bgHeader;
    position: relative;
    z-index: 1;
    &::before{
      content: "";
       opacity: 0.3;
      top: 0;
      left: 0;
      bottom: 0;
      right: 0;
      background-image: url(../assets/remote-training/images/waves.svg);
      position: absolute;
      z-index: -1;
    }
}

</style>