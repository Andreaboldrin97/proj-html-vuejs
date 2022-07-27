<template>
    <div class="d-flex ps-5">
        <div class="explore">
            <div class="title py-2">
                Explore
            </div>
            <div class="d-flex ">
                <div>
                    <listFooter v-for="(element , index) in explors" :key="index"
                            :item="element.item"
                            :itemUrl="element.itemUrl"/>
                </div>
            
                 <div>
                    <listFooter v-for="(element , index) in sections" :key="index"
                            :item="element.item"
                            :itemUrl="element.itemUrl"/>
                </div>
            </div>
        </div>

        <div class="information">
            <div class="title py-2 ">
                Information
            </div>
             <div class="">
                   <listFooter v-for="(element , index) in informations" :key="index"
                            :item="element.item"
                            :itemUrl="element.itemUrl"/>
                </div>
        </div>
        

       
    </div>
</template>

<script>
import listFooter from './listFooter.vue'


export default {
  components: { listFooter },
    
    data : function(){
        return{
            explors : [
                {
                    item : 'Start here',
                    itemUrl : '#'
                },
                {
                    item : 'Blog',
                    itemUrl : '#blog'
                },
                {
                    item : 'About us',
                    itemUrl : '#'
                }
            ],
            sections :[
                 {
                    item : 'Success strory',
                    itemUrl : '#success'
                },
                {
                    item : 'Courses',
                    itemUrl : '#courses'
                },
                {
                    item : 'Contact us',
                    itemUrl : '#'
                }
            ],
            informations : [
                 {
                    item : 'Membership',
                    itemUrl : '#'
                },
                {
                    item : 'Purchase guide',
                    itemUrl : '#'
                },
                {
                    item : 'Privacy policy',
                    itemUrl : '#'
                },
                {
                    item : 'Terms of services',
                    itemUrl : '#'
                }
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
.title {
  font-weight: 600;
}

</style>