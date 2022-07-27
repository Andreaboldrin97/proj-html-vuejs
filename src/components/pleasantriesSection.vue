
 <template>
    <div class="container pt-5">
        <div class="text-center">
            <div class="text-focus pb-3">
                WANNA TRANSFORM YOUR LIFE ?
            </div>
            <div class="service-help pb-3">
                Glad to <span class="blog-focus">Help You</span> Learn
            </div>
        </div>
        <div class="d-flex">
            <pleasantriesCard v-for="(element , index) in serviceCoursesHelp " :key="index"
                                :icon="element.icon"
                                :title="element.title"
                                :content="element.content"/>
        </div>
        <div class="hero-img position-relative">
            <img src="../assets/remote-training/images/home-6-services-image-1024x411.png" alt="">
        </div>
    </div>
</template>

<script>
import pleasantriesCard from './pleasantriesCard.vue' 

export default {

      components :{
         pleasantriesCard,
    },
    data : function(){
        return{
            serviceCoursesHelp : [
                {
                    icon : 'fa-brands fa-font-awesome',
                    title : 'Idea Discussion',
                    content : 'Get teamed up with the specialists who work and teach coding foe years at famous universities.'
                },
                {
                    icon : 'fa-solid fa-gear',
                    title : 'Web Development',
                    content : 'Lear to strat building a webpage from scratch. You decide your own pace, course and speed.'
                },
                {
                    icon : 'fa-solid fa-circle-nodes',
                    title : 'System Administration',
                    content : 'Learners are encouraged to study the mechanism and structure of system administartion.'
                },
                {
                    icon : 'fa-solid fa-display',
                    title : 'Graphic Design',
                    content : 'Have a passion for graphics and arts? Show talents with confidence and self-assertiveness.'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.text-focus{
    font-weight: 200;
}
.service-help{
    font-size: 40px;
    .blog-focus{
        color: $colorBreand;
        font-weight: 200;
    }
}
.hero-img{
    top: 35px;
    img{
        width: 100%;
        object-fit: cover;
    }
}

</style>