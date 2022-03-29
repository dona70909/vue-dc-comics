<template>
    <div class="my-main-content-menu padding">
        <div class="my-main-nav">
            <ul class="d-flex my-link-list" >
                <li class="my-link-item d-flex" v-for="(link,index) in headerLinks" :key="index" >

                    <img :src="link.image" />
                    <div class="my-link-text-wrap">
                        <p>{{link.text}}</p>
                    </div>      
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: "MainContentMenuDc",

    data(){
        return{
            headerLinks:[

                {text:"Digital Comics", url:"#", image:require('@/assets/img/buy-comics-digital-comics.png')},
                {text:"Dc Merchandise",  url:"#",  image:require('@/assets/img/buy-comics-merchandise.png')},
                {text:"Subscription",  url:"#",  image:require('@/assets/img/buy-comics-shop-locator.png')},
                {text:"Comic Shop Locator",  url:"#",  image:require('@/assets/img/buy-comics-subscriptions.png')},
                {text:"Dc Power Visa",  url:"#", image:require('@/assets/img/buy-dc-power-visa.svg')},
            ]
        }
    }
}
</script>

<style lang="scss" sccoped> 
    .my-main-content-menu{
        background-color:rgb(2, 130, 249);
        height: 150px;
    
        .my-main-nav{
            padding-top:3rem;

        
        }
    }

    .my-link-list{
        list-style-type:none;
        margin: 0;
        justify-content: space-around;

        .my-link-item{
            height: 50px;
            width: calc(100% / 5 - 1rem);
            border-bottom: transparent;

            img{
                margin-right:1rem;
                widows: 50%;
            }

            .my-link-text-wrap{
                display: flex;
                align-items: center;
                margin-right:1rem;
                text-transform: uppercase;
                color: white;
            }
        }
    }

</style>