<template>
    <div class="container">
        <div class="testimony-text py-5 text-center">
              Why People Talk About
              <span class="brand-name">MaxCoach</span>
              ?
        </div>

        <profileTestimony/>

        <div class="d-flex justify-content-evenly container-company">
             <companyTestimony  v-for="(element, index ) in companys" :key="index"
                                :name="element.name"
                                :imgCompany="element.imgCompany"    />
        </div>
       
    </div>
</template>

<script>
import profileTestimony from './profileTestimony.vue' 
import companyTestimony from './companyTestimony.vue' 

export default {
      components :{
         profileTestimony,
         companyTestimony
    },
    data : function(){
        return{
            companys : [
                {
                    name : 'aqua-Company',
                    imgCompany : 'client-logo-colored-01.png'
                },
                {
                    name : 'adroll-Company',
                    imgCompany : 'client-logo-colored-02.png'
                },
                {
                    name : 'firefox-Company',
                    imgCompany : 'client-logo-colored-03.png'
                },
                {
                    name : 'woodland-Company',
                    imgCompany : 'client-logo-colored-04.png'
                },
                {
                    name : 'bulfitt-Company',
                    imgCompany : 'client-logo-colored-05.png'
                },
                {
                    name : 'sixbase-Company',
                    imgCompany : 'client-logo-colored-06.png'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "./src/style/variables.scss";

.testimony-text{
    font-size: 45px;
    font-weight: 600;
    .brand-name{
        color: $colorBreand;
        font-weight: 200;
    }
}
.container-company{
    margin-top: 70px;
}
</style>
