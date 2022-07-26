<template>
  <div class="container py-5">
      <div class="text-center">
          <div class="text-focus pb-3">
              CHOOSE A COURSE TO GET STARTED
          </div>
          <div class="service-clients pb-3">
              Latest Featured <span class="service-text">Course</span>
          </div>
      </div>

      <div class="d-flex flex-wrap container-card">
          <courseCard v-for="(element,index) in courses" :key="index"
                    :imgCourse="element.imgCourse"
                    :price="element.price"
                    :courseContent="element.courseContent"
                    :lessons="elementlessons"
                    :students="element.students"/>
      </div>
      <div class="text-center">
          <btnForm class="pt-5"
            :btnFocus ="btnText.btnFocus"
            :btnLink="btnText.btnLink"
            />
      </div>
      
      
  </div>
</template>

<script>
import courseCard from './courseCard.vue' 
import btnForm from './btnForm.vue' 

export default {
          components :{
         courseCard,
         btnForm
    },
    data : function(){
        return{
            courses : [
                {
                    imgCourse : 'course-02-480x298.jpg',
                    price : '$40',
                    courseContent : 'Learning to write as a Professional Author',
                    lessons : 20,
                    students : 50
                },
                {
                    imgCourse : 'stock-full-hd-03-480x298.jpg',
                    price : 'Free',
                    courseContent : 'Costumer-centric Info-Tech Strategies',
                    lessons : 24,
                    students : 769
                },
                {
                    imgCourse : 'stock-full-hd-04-480x298.jpg',
                    price : '$19',
                    courseContent : 'Open Programmng Courses for Everyone: Python',
                    lessons : 17,
                    students : 62
                },
                {
                    imgCourse : 'stock-full-hd-06-480x298.jpg',
                    price : '$26',
                    courseContent : 'Academic Listening Note-taking',
                    lessons : 14,
                    students : 67
                },
                {
                    imgCourse : 'course-featured-image-01-480x298.jpg',
                    price : '$39',
                    courseContent : 'Master jQuery in a Short Period of Time',
                    lessons : 6,
                    students : 51
                },
                {
                    imgCourse : 'stock-full-hd-05-480x298.jpg',
                    price : '$59',
                    courseContent : 'Introduction to Javascript for Begginners',
                    lessons : 14,
                    students : 76
                }
            ],
            btnText :{
                    btnFocus : 'View all courses →',
                    btnLink : '#'
            }
            
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
.container-card{
    width: 80%;
    margin: 0 auto;
}
.text-focus{
    font-weight: 200;
}
.service-clients{
    font-size: 40px;
    .service-text{
        color: $colorBreand;
        font-weight: 200;
    }
}

</style>