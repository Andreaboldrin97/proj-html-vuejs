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

      <section>
          <testimony/>
      </section>
      
      <section class="blog">
          <sectionBlog/>
      </section>

      <section>
          <pleasantriesSection/>
      </section>
  </main>
</template>

<script>
import infoCourse from './infoCourse.vue' 
import statiscCard from './statiscCard.vue' 
import professionalSection from './professionalSection.vue' 
import sectionPrice from './sectionPrice.vue' 
import testimony from './testimony.vue' 
import sectionBlog from './sectionBlog.vue' 
import pleasantriesSection from './pleasantriesSection.vue' 

export default {
      components :{
         infoCourse,
         statiscCard,
         professionalSection,
         sectionPrice,
         testimony,
         sectionBlog,
         pleasantriesSection
    },
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
.info{
    background-image: url('../assets/remote-training/images/background-pattern-grid-line.png');
}
.price {
    margin-top: 150px ;
    background-color: $bgSectionPrice;
}
.blog{
    margin-top: 70px ;
    background-color: $bgSectionPrice;
}
</style>