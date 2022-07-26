<template>
  <div class="container d-flex border-r mt-5">

    <div class="card-container d-flex w-50 border-r">
        <div>
          <professionalCard/>
          <professionalCard2/>
          
        </div>
        <div class="position-relative second-card">
          <professionalCard/>
          <professionalCard2/>
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
        professions : [
          {
            profession : 'Graphic Design',
            description : 'Have a passion for graphics and arts? Show talents with confidence and self-assertiveness'
          },
          {
            profession : '',
            description : 'Have a passion for graphics and arts? Show talents with confidence and self-assertiveness'
          },
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