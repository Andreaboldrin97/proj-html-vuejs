<template>
  <footer >
    <div class="container"> 
      <div class="d-flex pt-5 ps-5">
          <div class="w-50">

            <div class="title py-2">
              Address
            </div>
            <div class="brand-info">
                <div class="py-1">
                  382 NE 191st ST # 87294 Miami, FL 33179-3899
                </div>
                <div class="py-1">
                  +1(305)547-9909 (9am - 5pm EST, Monday - Friday)
                </div>
                <div class="py-1 mail-brend">
                  <a href= "mailto:support@maxcoach.com">support@maxcoach.com</a>
                </div>
            </div>

            <div class="d-flex">
              <socialSection v-for="(element , index) in socials" :key="index"
                              :socialIcon="element.socialIcon"
                              :socialLink="element.socialLink"/>
            </div>
            
          </div>
          
          <div class="w-50">
            <informationSection/>
          </div>
      </div>
      <div class="text-center py-5 copyright-text">
        © 2020 Maxcoach. All Rights Reserved
      </div>
    </div>
  </footer>
</template>

<script>
import socialSection from './socialSection.vue' 
import informationSection from './informationSection.vue' 

export default {
  components : {
    socialSection,
    informationSection
  },
  data : function(){
    return{
      socials:[
        {
          socialIcon : 'fa-brands fa-facebook',
          socialLink :'#'
        },
        {
          socialIcon: 'fa-brands fa-twitter',
          socialLink :'#'
        },
        {
          socialIcon :'fa-brands fa-instagram',
          socialLink :'#'
        },
        {
          socialIcon : 'fa-brands fa-linkedin',
          socialLink :'#'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

footer{
  margin-top: 100px;
  background-color: $bgSectionligth ;
}
.title {
  font-weight: 600;
}
.brand-info{
  color: $footerText;
  .mail-brend{
    a{
      text-decoration: none;
      color: $footerText;
    }
  }
}
.copyright-text{
  color: $colorTextFocus;
}
</style>