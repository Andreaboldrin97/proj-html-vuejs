<template>
  <main>
      <section class="info position-relative" id="success">
            <infoCourse/>
            <statiscCard/>
            <professionalSection/>

            <div class="position-absolute c1"></div>
            <div class="position-absolute c2"></div>
            <div class="position-absolute c3"></div>
            <div class="position-absolute c4"></div>
            <div class="position-absolute c5"></div>

      </section>

      <section class="price" id="courses">
          <sectionPrice/>
      </section>

      <section>
          <testimony/>
      </section>
      
      <section class="blog" id="blog">
          <sectionBlog/>
      </section>

      <section class="pleasantries position-relative">
          <pleasantriesSection/>

            <div class="position-absolute c1"></div>
            <div class="position-absolute c2"></div>
            <div class="position-absolute c3"></div>
            <div class="position-absolute c4"></div>
            <div class="position-absolute c5"></div>
            
      </section>

      <section class="position-relative">
          <sectionStartedBanner />

            <div class="position-absolute c2"></div>
            <div class="position-absolute c3"></div>
            <div class="position-absolute c4"></div>
            <div class="position-absolute c5"></div>
      </section>
  </main>
</template>

<script>
import infoCourse from './mainComponents/sectionINFO/infoCourse.vue' 
import statiscCard from './mainComponents/sectionINFO/statiscCard.vue' 
import professionalSection from './mainComponents/sectionINFO/professionalSection.vue' 
import sectionPrice from './mainComponents/sectionPRICE/sectionPrice.vue' 
import testimony from './mainComponents/sectionTESTIMONY/testimony.vue' 
import sectionBlog from './mainComponents/sectionBLOG/sectionBlog.vue' 
import pleasantriesSection from './mainComponents/sectionPLEASANTIES/pleasantriesSection.vue' 
import sectionStartedBanner from './mainComponents/sectionBANNER/sectionStartedBanner.vue' 

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



// circle content
.c1{
    width: 20px;
    height: 20px;
    border-radius: 50%;
    background-color: $circlered;
    top: 2%;
    left: 27%;
    
}
.c2{
    width: 30px;
    height: 30px;
    border-radius: 50%;
    background-color: $circlePink;
    top: 10%;
    opacity: 0.5;
    left: 50%;
    z-index: -1;
}
.c3{
    width: 10px;
    height: 10px;
    border-radius: 50%;
    background-color: $bgBtnHover ;
    top: 5%;
    right: 30%;
}
.c4{
    width: 25px;
    height: 25px;
    border-radius: 50%;
    background-color: $circleYellow;
    top: 13%;
    right: 18%;
}
.c5{
    width: 35px;
    height: 35px;
    border: 5px solid $colorBreand;
    border-radius: 50%;
    background-color: white;
    top: 5%;
    left: 19%;
}
</style>