<template>
   <div class="w-50 ms-5 align-self-center">
        <div class="text-focus pb-3">
            TOGETHER WE CAN CREATE
        </div>
        <div class="service-clients pb-3">
          Service We <span class="service-text">Can Provide</span> For My Clients.
        </div>
        <div class="list-service py-1" v-for="(element,index) in clientsServis" :key="index">
             <i class="fa-solid fa-check pe-3"></i> {{ element }}
        </div>
        <a :href="btnLink" class="btn btn_focus text-white px-4 mt-3"> Get started for free</a>
    </div>
</template>

<script>
export default {
    data : function(){
        return{
            clientsServis : [
                'Select & customize courses to your preferences',
                'Change the tutor and make arrangements',
                'Participate in events to join others',
                'Get the desired certificate delivered at house'
            ]
        }
    }

}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
.text-focus{
    font-weight: 200;
}
.service-clients{
    font-size: 35px;
    .service-text{
        color: $colorBreand;
        font-weight: 200;
    }
}
.list-service{
    font-size: 12px;
    font-weight: 300;
    i{
        color: $colorBreand;
    }
}
.btn_focus{
    background-color: $colorBreand;
}
</style>