//! card delle professioni che offre il sito ( al cambio di un valore ca,bia la posizione delle img)
<template>
  <div class="professional-card m-3 my-3 px-2 d-flex flex-column justify-content-between " :class="isReverse  ? 'flex-column-reverse' : '' ">
        <div class="p-2 img-text-card">
                <div class="text-title pt-3">{{ profession }}</div>
                <div class="text-description pt-1">
                  {{ description }}
                </div>
        </div>
        <div class="img-card">
           <img :src="require(`@/assets/remote-training/images/${img}`)" :alt="profession">
        </div>
    </div>
</template>

<script>
export default {
    props:{
        profession : String,
        description : String,
        img : String,
        isReverse : Boolean
    }
}
</script>

<style lang="scss" scoped>


.professional-card{
  box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
  img{
    width: 100%;
    height: 200px;
    object-fit: contain;
    object-position: left;
  }
  .text-title{
    font-size: 20px;
    font-weight: 500;
  }
  .text-description{
    font-size: 20px;
    font-weight: 300;
  }
}

</style>