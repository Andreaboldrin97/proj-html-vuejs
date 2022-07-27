<template>
    <div class="pe-5">
        <div class="py-1">
            <a :href="itemUrl">
                {{ item }}
            </a>
        </div>
    </div>
</template>

<script>
export default {
    props :{
        item : String,
        itemUrl : String
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
a{
    text-decoration: none;
    color: $footerText;
}

</style>