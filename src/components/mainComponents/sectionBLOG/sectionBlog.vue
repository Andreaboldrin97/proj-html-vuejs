<template>
  <div class="container py-5">
       <div class="text-center">
          <div class="text-focus pb-3">
              ENJOY READING ON MAXCOACH
          </div>
          <div class="service-blog pb-3">
              Latest On <span class="blog-focus">Our Blogs</span>
          </div>
      </div>

      <div class="d-flex pb-5">
          <cardBlog v-for="(element,index) in blogsForm" :key="index"
                    :imgBlog ="element.imgBlog"
                    :blogGenre ="element.blogGenre"
                    :blogContent ="element.blogContent"
                    :date ="element.date"
                    :views ="element.views" />
      </div>
      
  </div>
</template>

<script>
import cardBlog from './cardBlog.vue' 

export default {

      components :{
         cardBlog,
    },

    data : function(){
        return{
             blogsForm : [
                {
                    imgBlog : 'artist-blog-03-480x325.jpeg',
                    blogGenre : 'ARTIST',
                    blogContent : 'Brush Stokes Energize Trees in Paintings',
                    date : 'May 15,2020',
                    views : 688
                },
                {
                    imgBlog : 'artist-blog-01-480x325.jpg',
                    blogGenre : 'ARTIST',
                    blogContent : 'Pocket-Sized Notebooks Hold Miniature Paintings',
                    date : 'May 15,2020',
                    views : 603
                },
                {
                    imgBlog : 'artist-blog-02-480x325.jpg',
                    blogGenre : 'ARTIST',
                    blogContent : 'Connection Between Self-Portrats and Identity',
                    date : 'May 15,2020',
                    views : 397
                },
                ]
        }
    },
}
</script>

<style lang="scss" scoped>
@import "./src/style/variables.scss";
.container-card{
    width: 80%;
    margin: 0 auto;
}
.text-focus{
    font-weight: 200;
}
.service-blog{
    font-size: 40px;
    .blog-focus{
        color: $colorBreand;
        font-weight: 200;
    }
}

</style>