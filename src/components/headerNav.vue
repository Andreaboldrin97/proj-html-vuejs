<template>
   <nav class="container m-auto p-2 d-flex">
            <div class="logo-img pe-5 align-items-center d-flex">
                <img src="../assets/remote-training/images/light-logo.png" alt="">
            </div>
            <div class="container-nav d-flex justify-content-evenly align-items-center">
                <div class="nav-links" v-for="(element , index) in linksNav" :key="index">
                   <a :href="linkUrl"> {{ element.linkName }} <span><i class="fa-solid fa-chevron-down"></i></span></a>
                </div>
                <div class="d-flex icon-user">
                    <i class="fa-solid fa-cart-shopping pe-3"></i>
                    <i class="fa-regular fa-circle-user"></i>
                </div>
            </div>
            <div class="search-bar">
                <div class="input-group">
                    <input type="text" class="form-control" placeholder="Search" v-model.trim="searchInput">
                    <span class="input-group-text"><i class="fa-solid fa-magnifying-glass"></i></span>
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

<style lang="scss" scopped>
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
    i{
        font-size: 12px;
        vertical-align: middle;
    }
}
.search-bar{
    width: 20%;
}
</style>