<template>
  <div class="container d-flex mt-5">

    <div class="card-container d-flex w-50 ">
        <div>
          <professionalCard v-for="(element,index) in graphicProfession" :key="index"
                          :profession="element.profession"
                          :description="element.description"
                          :img="element.img"
                          :isReverse="element.isReverse"/>
          <professionalCard v-for="(element,index) in discussionProfession" :key="index"
                          :profession="element.profession"
                          :description="element.description"
                          :img="element.img"
                          :isReverse="element.isReverse"/>
          
        </div>
        <div class="position-relative second-card">
          <professionalCard v-for="(element,index) in businessProfession" :key="index"
                          :profession="element.profession"
                          :description="element.description"
                          :img="element.img"
                          :isReverse="element.isReverse"/>
          <professionalCard v-for="(element,index) in developmentProfession" :key="index"
                          :profession="element.profession"
                          :description="element.description"
                          :img="element.img"
                          :isReverse="element.isReverse"/>
        </div>
    </div>
    
    
   <serviceCard/>
  </div>
</template>

<script>
import professionalCard from './professionalCard.vue' 
import serviceCard from './serviceCard.vue' 

export default {
    components :{
          professionalCard,
          serviceCard
    },
    data : function(){
      return{
        graphicProfession : [
          {
            profession : 'Graphic Design',
            description : 'Have a passion for graphics and arts? Show talents with confidence and self-assertiveness.',
            img : 'home-6-service-image-01.png',
            isReverse : false
          }
        
        ],
        businessProfession : [
           {
            profession : 'Business Administration',
            description : 'Learnes are encouraged to study the mechanism and structure of system administration.',
            img : 'home-6-service-image-02.png',
            isReverse : false
          }
        ],
        discussionProfession : [
           {
            profession : 'Idea Discussion',
            description : 'Get teamed up with the specialists who work and teach coding for years at famous universities.',
            img : 'home-6-service-image-03.png',
            isReverse : true
          },
        
        ],
        developmentProfession : [
            {
            profession : 'Web development',
            description : 'Learn to start building a webpage from scratch. You decide your own pace, course and speed.',
            img : 'home-6-service-image-04.png',
            isReverse : true
          }
        ]
      }
    }
}
</script>

<style lang="scss" scoped>
.second-card{
  top: 10%;
}
</style>