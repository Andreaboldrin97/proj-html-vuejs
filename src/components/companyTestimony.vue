   //! conponents per le compagnie affiliate usato in testimony.vue
<template>
      <div class="container-company">
          <img :src="require(`../assets/remote-training/images/${imgCompany}`)" :alt="name">
      </div>
</template>

<script>
export default {
    props:{
        name : String,
        imgCompany : String
    }
}
</script>

<style lanf="scss" scoped>
img{
    width: 100%;
}

</style>