<template>
    <div class="blog-card">
        <div >
            <img class="rounded" :src="require(`@/assets/remote-training/images/${imgBlog}`)" alt="img-blog"> 
        </div>
        <div class="text-card">
            <div class="genre py-3">
                {{ blogGenre }}
            </div>
            <div class="blog-title pb-4">
                {{ blogContent }}
            </div>
            <div class="d-flex blog-views">
                <div class="pe-5">
                    <i class="fa-regular fa-calendar pe-2"></i>
                        {{ date }}
                </div>
                <div>
                    <i class="fa-regular fa-eye"></i>
                      {{ views }}  views
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props : {
            imgBlog : String,
            blogGenre : String,
            blogContent : String,
            date : [Number,String],
            views : [Number,String]
        }
}


</script>

<style lang="scss" scoped>
@import "./src/style/variables.scss";

.blog-card {
    cursor: pointer;
    width: calc((100vw / 3) - 30px);
    margin: 15px;
    img{
        width: 100%;
    }
}
.text-card{
    .genre{
        color: $colorTextFocus;
        font-weight: 400;
    }
    .blog-title{
        font-size: 22px;
        font-weight: 600;
    }
    .blog-views{
        color: $colorTextFocus;
    }
}
</style>
