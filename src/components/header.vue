<template>
  <header class="hero-header">
    <headerNav/>
    <heroHeaderMessage/>
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
  

}
</script>

<style lang="scss" scooped>
.hero-header{
    background-color: #1f2154;
}

</style>