<template>
   <nav class="container m-auto p-2 d-flex">
            <div class="logo-img pe-5 align-items-center d-flex">
                <img src="@/assets/remote-training/images/light-logo.png" alt="logo-img">
            </div>
            <div class="container-nav d-flex justify-content-evenly align-items-center">
                <div class="nav-links" v-for="(element , index) in linksNav" :key="index">
                   <a :href="linkUrl"> {{ element.linkName }} <span><i class="fa-solid fa-chevron-down"></i></span></a>
                </div>
                <div class="d-flex icon-user align-items-center">
                    <div class="position-relative pe-3">
                        <i class="fa-solid fa-cart-shopping"></i>
                        <span class="shopping-items position-absolute">
                            <span class="number-shop-list position-absolute">0</span>
                        </span>
                    </div>
                    
                    <i class="fa-regular fa-circle-user"></i>
                </div>
            </div>
            <div class="search-bar">
                <div class="input-group">
                    <input type="text" class="form-control" placeholder="Search" v-model.trim="searchInput">
                    <span class="input-group-text icon-container"><i class="fa-solid fa-magnifying-glass"></i></span>
                </div>
            </div>
      </nav>
</template>

<script>
export default {
      data : function(){
        return {
            searchInput : '',
            linksNav : [
                {
                    linkName : 'Home',
                    linkUrl : '#'
                },
                {
                    linkName : 'Pages',
                    linkUrl : '#'
                },
                {
                    linkName : 'Counses',
                    linkUrl : '#'
                },
                {
                    linkName : 'Features',
                    linkUrl : '#'
                },
                {
                    linkName : 'Blog',
                    linkUrl : '#'
                },
                {
                    linkName : 'shop',
                    linkUrl : '#'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "./src/style/variables.scss";

.logo-img{
    width: 20%;
    img{
        width: 100%;
    }
}
.container-nav{
    width: 75%;
    color: white;
}
.nav-links{
    cursor: pointer;
    i{
        font-size: 12px;
        vertical-align: middle;
    }
}
.search-bar{
    width: 20%;
    .icon-container{
        background-color: white;
    }
    i{
        color: $colorBreand;
        
    }
}
.icon-user{
    font-size: 20px;
    cursor: pointer;

    .shopping-items{
    width: 15px;
    height: 15px;
    color: black;
    background-color: white;
    border-radius: 50%;
    top: -5%;
    left : 40%;
    }
    .number-shop-list{
        font-size: 12px;
        top: -10%;
        left: 22%;
    }
}

</style>