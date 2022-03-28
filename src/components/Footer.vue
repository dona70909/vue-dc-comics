<template>
    <div class="my-footer-wrap">

        <div class="my-footer-container-links d-flex padding position-relative">
            <div class="my-footer-nav d-flex">
                <ul>
                    <li><h4>Dc Comics</h4></li>
                    <li v-for="(link,index) in linkFooterComics" :key="index">
                        {{link.text}}
                    </li>
                </ul>

                <ul>
                    <li><h4>Dc </h4></li>
                    <li v-for="(link,index) in linkFooterDc" :key="index">
                        {{link.text}}
                    </li>
                </ul>

                <ul>
                    <li><h4>Dc </h4></li>
                    <li v-for="(link,index) in linkFooterDc" :key="index">
                        {{link.text}}
                    </li>
                </ul>

                <ul>
                    <li><h4>Sites</h4></li>
                    <li v-for="(link,index) in linkFooterSites" :key="index">
                        {{link.text}}
                    </li>
                </ul>

                <ul>
                    <li><h4>Shop</h4></li>
                    <li v-for="(link,index) in linkFooterShop" :key="index">
                        {{link.text}}
                    </li>
                </ul>


            </div>

            <div class="my-footer-bg-image">
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </div>

        </div>


        

    </div>
</template>

<script>
export default {
    name: "FooterDc",
    data(){
        return{
            linkFooterComics:[
                {text:"Characters", url:"#"},
                {text:"Comics", url:"#"},
                {text:"Movies", url:"#"},
                {text:"Tv", url:"#"},
                {text:"Games", url:"#"},
                {text:"Videos", url:"#"},
                {text:"News", url:"#"},
            ],

            linkFooterDc:[
                {text:"Characters", url:"#"},
                {text:"Comics", url:"#"},
                {text:"Movies", url:"#"},
                {text:"Tv", url:"#"},
                {text:"Games", url:"#"},
                {text:"Videos", url:"#"},
                {text:"News", url:"#"},
                {text:"Games", url:"#"},
                {text:"Videos", url:"#"},
                {text:"News", url:"#"},
            ],
            linkFooterSites:[
                {text:"Characters", url:"#"},
                {text:"Comics", url:"#"},
                {text:"Movies", url:"#"},
                {text:"Tv", url:"#"},
                {text:"Tv", url:"#"},
            ],
            linkFooterShop:[
                {text:"Characters", url:"#"},
                {text:"Comics", url:"#"},
            ],  

            
        }
    }
}
</script>

<style lang="scss" scoped>
.my-footer-wrap{
    background-image:url("../assets/img/footer-bg.jpg");
    height: 350px;
}

.my-footer-nav{
    width:50%;
    justify-content: space-around;
    padding-top:2rem;
    flex: wrap;
    flex-shrink: none;  

    ul{
        list-style: none;

        h4{
            text-transform:uppercase;
            color: white;
        }

        li{
            padding: .3rem;
            color: rgb(192, 188, 184);
            
        }
    }
}

.my-footer-bg-image{
    height: 400px;
    width:30%;
    top: -2rem;
    right: 200px;
    position:absolute;

    img{
        height: 100%;
        width: 100%;
    }
}


</style>