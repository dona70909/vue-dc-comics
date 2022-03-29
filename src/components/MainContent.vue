<template>
    <div class="my-main-wrapper position-relative">

        <div class="box-current-series">
            <h4>Current Series</h4>
        </div>
        <div class="main-content-cards ">
            <div v-for="(card,index) in mainCards" :Key="index" class="main-card">
                <img :src="card.thumb" alt="">
                <p>{{card.series}}</p>
            </div>
        </div>

        <div class="button-wrapper">
            <button class="load-more-btn"><a href="#">Load more</a></button>
        </div>
    </div>
</template>

<script>
export default {
    name:"MainContentDc",
    data(){
        return{

            mainCards : [

                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]
        }
    }

}
</script>

<style lang="scss" scoped>
.my-main-wrapper{
    width: 100%;
    padding:0;
    background-color: black;

    .main-content-cards{   
        width: 100%; 
        justify-content: center;
        padding: 4rem 8rem;
        display: flex;
        flex-wrap: wrap;
        gap: 1rem 2rem;
        background-color: black;
        .main-card{
            height: 300px;
            width: calc(100% / 6 - 2rem);
            color: white;
            display: flex;
            flex-direction: column;

            img{
                width: 100%;
                height:80%;
                padding-bottom: 1rem
            };

            p{
                text-transform: uppercase;
                text-align: center;
            }
        }
    }

    .button-wrapper{
        display: flex;
        justify-content: center;
        padding-bottom: 1rem ;

        button{
        background-color: rgb(2, 130, 249);
        padding: 1rem;
        border: none;
        
            a{
                text-decoration: none;
                color: white;
                text-transform: uppercase;
                font-weight: 700;
            }
        }
    }

    .box-current-series{
        padding: 1rem;
        height: 50px;
        width: 200px;
        background-color: rgb(2, 130, 249);
        position: absolute;
        top: -1rem;
        left: 5rem;
        h4{
            color: white;
            text-transform: uppercase;
            font-weight: 700;
            text-align: center;
            line-height:25px;
        }
    }
}
</style>