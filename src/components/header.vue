<template>
  <header class="hero-header">
    <headerNav/>
    <heroHeaderMessage v-for="(element, index) in focusMessage" :key="index"
                :focus="element.focus"
                :textInfo ="element.textInfo "
                :btnFocus="element.btnFocus"
                :btnLink="element.btnLink"/>
    
  </header>
</template>

<script>
import headerNav from './headerNav.vue' 
import heroHeaderMessage from './heroHeaderMessage.vue' 

export default {
     components :{
         headerNav,
        heroHeaderMessage,
    },
     data : function (){
        return{
            focusMessage : [{
                focus : 'Learn At Own Pace!',
                textInfo : 'Get teamed up whith peoople of the same will.',
                btnFocus :'Get started for free',
                btnLink : '#'
            }]
        }
    }

}
</script>

<style lang="scss" scooped>
.hero-header{
    background-color: #1f2154;
}

</style>