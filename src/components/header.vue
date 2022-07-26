<template>
  <header class="hero-header">
    <headerNav/>
    <heroHeaderMessage v-for="(element, index) in focusMessage" :key="index"
                :focus="element.focus"
                :textInfo ="element.textInfo "
                :btnFocus="element.btnFocus"
                :btnLink="element.btnLink"/>
    <heroBanner/>
  </header>
</template>

<script>
import headerNav from './headerNav.vue' 
import heroHeaderMessage from './heroHeaderMessage.vue' 
import heroBanner from './heroBanner.vue' 

export default {
     components :{
         headerNav,
        heroHeaderMessage,
        heroBanner
    },
     data : function (){
        return{
            focusMessage : {
                focus : 'Learn At Own Pace!',
                textInfo : 'Get teamed up whith peoople of the same will.',
                btnFocus :'Get started for free',
                btnLink : '#'
            }
        }
    }

}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
.hero-header{
    background-color: $bgHeader;
}

</style>