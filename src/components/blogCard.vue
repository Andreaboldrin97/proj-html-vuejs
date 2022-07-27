<template>

    <div class="blog-card">
        <div>
            <img class="rounded" src="../assets/remote-training/images/artist-blog-01-480x325.jpg" alt="">
        </div>
        <div class="text-card">
            <div class="genre py-3">
                ARTIST
            </div>
            <div class="blog-title pb-4">
                Pocket-Sized Notebooks Hold Miniature Paintings
            </div>
            <div class="d-flex blog-views">
                <div class="pe-5">
                    <i class="fa-regular fa-calendar pe-2"></i>
                        May 15,2020
                </div>
                <div>
                    <i class="fa-regular fa-eye"></i>
                        views
                </div>
            </div>
        </div>
    </div>
     

</template>

<script>

</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
.blog-card {
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
        font-size: 20px;
        font-weight: 700;
    }
    .blog-views{
        color: $colorTextFocus;
    }
}
</style>