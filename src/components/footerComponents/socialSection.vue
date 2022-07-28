<template>

    <div class="py-4 pe-3 social-item">
        <a :href="socialLink">
            <i :class="socialIcon"></i>
        </a>
    </div>
 
</template>

<script>
export default {
    props :{
        socialIcon : String,
        socialLink : String
    }

}
</script>

<style lang="scss" scoped>
@import "./src/style/variables.scss";

.social-item{
    font-size: 25px;
    a{
        color: $colorTextFocus;
    }
    
}
</style>