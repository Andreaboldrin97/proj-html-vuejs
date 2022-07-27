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

      <section class="pleasantries">
          <pleasantriesSection/>
      </section>

      <section>
          <sectionStartedBanner/>
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
import sectionStartedBanner from './sectionStartedBanner.vue' 

export default {
      components :{
         infoCourse,
         statiscCard,
         professionalSection,
         sectionPrice,
         testimony,
         sectionBlog,
         pleasantriesSection,
         sectionStartedBanner
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
    background-color: $bgSectionligth ;
}
.blog{
    margin-top: 70px ;
    background-color: $bgSectionligth ;
}
.pleasantries{
   background: rgb(236,236,238);
    background: linear-gradient(0deg, rgb(219, 218, 218) 0%, rgba(255,255,255,1) 43%);
}
</style>