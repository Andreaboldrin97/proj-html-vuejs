<template>
  <div class="professional-card m-2 my-3 px-2">
        <div class="p-2">
                <div>{{ profession }}</div>
                <div class="text-description pt-1">
                  {{ description }}
                </div>
        </div>
         <img :src="require(`../assets/remote-training/images/${img}`)" :alt="profession">
    </div>
</template>

<script>
export default {
    props:{
        profession : String,
        description : String,
        img : String
    }
}
</script>

<style lang="scss" scoped>


.professional-card{
  box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
  img{
    width: 100%;
  }
  .text-description{
    font-size: 12px;
    font-weight: 300;
  }
}

</style>