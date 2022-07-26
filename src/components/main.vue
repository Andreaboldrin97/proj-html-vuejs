<template>
  <section>
      <section>
            <infoCourse/>
            <statiscCard/>
            <professionalCard/>
      </section>
  </section>
</template>

<script>
import infoCourse from './infoCourse.vue' 
import statiscCard from './statiscCard.vue' 
import professionalCard from './professionalCard.vue' 

export default {
      components :{
         infoCourse,
         statiscCard,
         professionalCard
       
    },
}
</script>

<style>

</style>