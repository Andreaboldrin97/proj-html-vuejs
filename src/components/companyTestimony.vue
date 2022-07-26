<template>
      <div>
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


</style>