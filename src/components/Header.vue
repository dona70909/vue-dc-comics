<template>
    <div class="my-header-content d-flex padding">
        <div class="my-header-logo">
            <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <div class="my-header-nav">
            <ul class="d-flex my-link-list" >
                <li class="my-link-item" v-for="(link,index) in headerLinks" :key="index" >
                    <a :href="link.url">{{link.text}}</a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {

    name: "HeaderDc",

    data(){
        return{
            headerLinks:[

                {text:"Characters", url:"#"},
                {text:"Comics",  url:"#"},
                {text:"Movies",  url:"#"},
                {text:"Tv",  url:"#"},
                {text:"Games",  url:"#"},
                {text:"Collectibles",  url:"#"},
                {text:"Videos",  url:"#"},
                {text:"Fans",  url:"#"},
                {text:"News",  url:"#"},
                {text:"Shop",  url:"#"},
            ]
        }

    }

}
</script>

<style lang="scss" scoped>

.my-header-content{
    justify-content: space-between;
    padding-top:1rem;
    padding-bottom:1rem;

}

.my-header-nav{
    line-height: 106.5px;

    .my-link-list{
        list-style-type:none;
        margin: 0;

        .my-link-item{
            padding: .5rem;
            border-bottom: transparent;

            a{
                text-decoration: none;
                color:black;
                text-transform: uppercase;
                font-weight: 600;
                font-size: .8rem;
            }
        }
    }
}



</style>