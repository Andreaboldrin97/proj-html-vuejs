
 <template>
    <div class="container py-5">
        <div class="text-center">
            <div class="text-focus pb-3">
                WANNA TRANSFORM YOUR LIFE ?
            </div>
            <div class="service-help pb-3">
                Glad to <span class="blog-focus">Help You</span> Learn
            </div>
        </div>
        <div class="d-flex">
            <pleasantriesCard/>
        </div>
    </div>
</template>

<script>
import pleasantriesCard from './pleasantriesCard.vue' 

export default {

      components :{
         pleasantriesCard,
    },
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

</style>