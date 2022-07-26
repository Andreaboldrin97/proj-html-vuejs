<template>
  <main>
      <section class="info">
            <infoCourse/>
            <statiscCard/>
            <professionalSection/>
      </section>
  </main>
</template>

<script>
import infoCourse from './infoCourse.vue' 
import statiscCard from './statiscCard.vue' 
import professionalSection from './professionalSection.vue' 

export default {
      components :{
         infoCourse,
         statiscCard,
         professionalSection
       
    },
}
</script>

<style lang="scss">
.info{
    background-image: url('../assets/remote-training/images/background-pattern-grid-line.png');
}
</style>