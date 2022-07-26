<template>
  <main>
      <section class="info">
            <infoCourse/>
            <statiscCard/>
            <professionalSection/>
      </section>
      <section class="price">
          <sectionPrice/>
      </section>
  </main>
</template>

<script>
import infoCourse from './infoCourse.vue' 
import statiscCard from './statiscCard.vue' 
import professionalSection from './professionalSection.vue' 
import sectionPrice from './sectionPrice.vue' 

export default {
      components :{
         infoCourse,
         statiscCard,
         professionalSection,
       sectionPrice
    },
}
</script>

<style lang="scss">
@import "../style/variables.scss";
.info{
    background-image: url('../assets/remote-training/images/background-pattern-grid-line.png');
}
.price {
    margin-top: 150px ;
    background-color: $bgSectionPrice;
}
</style>