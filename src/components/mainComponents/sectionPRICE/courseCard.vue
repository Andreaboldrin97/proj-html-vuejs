//! creazione carta per i corsi disponibili in sectionPrice.vue
<template>
    <div class="d-flex container-course p-3">
        <div class="img-course me-4">
          <img :src="require(`@/assets/remote-training/images/${imgCourse}`)" alt="img-course">
        </div>
        <div class="align-self-center">
              <div class="pb-2 price-course">
                  {{ price }}<span class="price-rest">.00</span>
              </div>
              <div class="pb-2 course-content">
                  {{ courseContent }}
              </div>
              <div class="d-flex course-info">
                  <div class="pe-5">
                      <i class="fa-regular fa-file-lines pe-2"></i>
                      {{ lessons }} Lessons
                  </div>
                  <div>
                      <i class="fa-regular fa-user pe-2"></i>
                      {{ students }} Students
                  </div>
              </div>
        </div>
    </div>
</template>

<script>
export default {
  props : {
            imgCourse : String,
            price : [Number, String],
            courseContent : String,
            lessons : [Number, String],
            students : [Number, String],
  }

}
</script>

<style lang="scss" scoped>
@import "./src/style/variables.scss";

.container-course{
  width: 50%;
  margin: 25px 0;
  &:hover{
    background-color: white;
    border-radius: 10px;
  }
}
.img-course{
  img{
    width: 150px;
    height: 150px;
    object-fit: cover;
    border-radius: 50%;
  }
}
.price-course{
  color: $colorBreand;
  font-weight: 800;
  .price-rest{
    font-size: 13px;
  }
}
.course-content{
  font-weight: 600;
}
.course-info{
  color: $colorTextFocus;
}
</style>