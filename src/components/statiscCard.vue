<template>
  <div class="container d-flex justify-content-center statisc-container">
      <div class="mx-4 text-center" v-for="(element , index) in statiscContent" :key="index">
            <div class="statisc-number">
           {{ element.staticsNumber }}
            </div>
            <div class="statisc-text pt-1">
                {{ element.statiscText }}
            </div>
      </div>
  </div>
</template>

<script>
export default {
    data : function(){
        return{
            statiscContent: [
                {
                    staticsNumber : '1.926',
                    statiscText : 'FINISHED SESSIONS'
                },
                {
                    staticsNumber : '3.092+',
                    statiscText : 'ENROLLED LEARNERS'
                },
                {
                    staticsNumber : '200',
                    statiscText : 'ONLINE INSTRUCTORS'
                },
                {
                    staticsNumber : '100%',
                    statiscText : 'SATISFACTION RATE'
                }
            ]
        }
    }

}
</script>

<style lang="scss" scoped>
.statisc-container{
    margin-top: 100px;
    .statisc-number{
        font-size: 35px;
        font-weight: 700;
        color: #1fad96;
    }
    .statisc-text{
        font-size: 13px;
        font-weight: 300;
    }
}
</style>