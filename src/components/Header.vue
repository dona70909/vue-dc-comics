<template>
    <div class="my-header-content d-flex padding">
        <div class="my-header-logo">
            <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <div class="my-header-nav">
            <ul class="d-flex my-link-list" >
                <li class="my-link-item" v-for="(link,index) in headerLinks" :key="index">
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

                {text:"Characters", url:"#", active:false},
                {text:"Comics",  url:"#", active:false},
                {text:"Movies",  url:"#", active:false},
                {text:"Tv",  url:"#", active:false},
                {text:"Games",  url:"#", active:false},
                {text:"Collectibles",  url:"#", active:false},
                {text:"Videos",  url:"#", active:false},
                {text:"Fans",  url:"#", active:false},
                {text:"News",  url:"#", active:false},
                {text:"Shop",  url:"#", active:false},
            ],

            active:null
        }

    },

    methods: {
        getActiveIndex(index){
            this.headerLinks[index].active = true;
            this.active = index;
            console.log(this.headerLinks[index].active);
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
            padding:.5rem 1rem;
            a{
                text-decoration: none;
                color:black;
                text-transform: uppercase;
                font-weight: 600;
                font-size: .8rem;
                border-bottom:5px solid transparent;
                padding-bottom: 48px;
                
            }

            a:hover{
                border-bottom:5px solid rgb(2, 130, 249);
            }
        }
    }
}

</style>