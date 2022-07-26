<template>
  <div class="container d-flex border-r mt-5">

    <div class="card-container d-flex w-50 border-r">
        <div>
          <professionalCard v-for="(element,index) in graphicProfession" :key="index"
                          :profession="element.profession"
                          :description="element.description"
                          :img="element.img"/>
          <professionalCard2 v-for="(element,index) in discussionProfession" :key="index"
                          :profession="element.profession"
                          :description="element.description"
                          :img="element.img"/>
          
        </div>
        <div class="position-relative second-card">
          <professionalCard v-for="(element,index) in businessProfession" :key="index"
                          :profession="element.profession"
                          :description="element.description"
                          :img="element.img"/>
          <professionalCard2 v-for="(element,index) in developmentProfession" :key="index"
                          :profession="element.profession"
                          :description="element.description"
                          :img="element.img"/>/>
        </div>
    </div>
    
    
    <div class="w-50 border-r text-center align-self-center">
        <div>
          TOGHEDER WE CAN CREATE
        </div>
        <div>
          Service We <span>Can Provide</span> For My Clients.
        </div>
        <ol>
          <li>Select &amp; customize courses to your preferences</li>
          <li>Chenge the tutor and make arrangements</li>
          <li>Participate in events to join others</li>
          <li>Get the desired certificate deòivered at house</li>
        </ol>
        <a :href="btnLink" class="btn btn_focus text-white px-4"> Get started for free</a>
    </div>
  </div>
</template>

<script>
import professionalCard from './professionalCard.vue' 
import professionalCard2 from './professionalCard2.vue' 

export default {
    components :{
          professionalCard,
          professionalCard2
    },
    data : function(){
      return{
        graphicProfession : [
          {
            profession : 'Graphic Design',
            description : 'Have a passion for graphics and arts? Show talents with confidence and self-assertiveness.',
            img : 'home-6-service-image-01.png'
          }
        
        ],
        businessProfession : [
           {
            profession : 'Business Administration',
            description : 'Learnes are encouraged to study the mechanism and structure of system administration.',
            img : 'home-6-service-image-02.png'
          }
        ],
        discussionProfession : [
           {
            profession : 'Idea Discussion',
            description : 'Get teamed up with the specialists who work and teach coding for years at famous universities.',
            img : 'home-6-service-image-03.png'
          },
        
        ],
        developmentProfession : [
            {
            profession : 'Web development',
            description : 'Learn to start building a webpage from scratch. You decide your own pace, course and speed.',
            img : 'home-6-service-image-04.png'
          }
        ]
      }
    }
}
</script>

<style lang="scss" scoped>
.border-r {
  border: 1px solid red;
}
.btn_focus{
    background-color: #1fad96;
}
.second-card{
  top: 10%;
}
</style>