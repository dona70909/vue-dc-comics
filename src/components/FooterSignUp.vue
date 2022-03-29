<template>
    <div class="my-footer-sign-up d-flex padding position-relative">
        <div>
            <button><a href="#">Sign-up now</a></button>
        </div>

        <div class="d-flex my-social-wrapper">
            <a href="#">Follow us</a>
            
            <ul class="d-flex">
                <li v-for="(img,index) in socialImages" :key="index">
                    <img :src="img.image" alt="">
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name:"FooterSignUpDc",
    data(){
        return{
            socialImages:[
                { image:require('@/assets/img/footer-facebook.png')},
                { image:require('@/assets/img/footer-periscope.png')},
                { image:require('@/assets/img/footer-pinterest.png')},
                { image:require('@/assets/img/footer-twitter.png')},
                { image:require('@/assets/img/footer-youtube.png')},
                
            ]
        }
    }
}
</script>

<style lang="scss" scoped>

.my-footer-sign-up{
    justify-content: space-between;
    height: 100px;
    background: rgb(48, 48, 48);
    z-index: 2;
    padding-top: 2rem;

    .footer-social-wrapper{
        align-items: center;
    }

    button{
        padding: 1rem;
        border-color:rgb(24, 123, 216);
        background: transparent;
        a{
            color: white;
            text-transform: uppercase;
            font-weight: 600;
            color: rgb(24, 123, 216);
        }
    }

    .my-social-wrapper{
        li{
            padding:0 .5rem;
        }

        a{
            line-height: 30px;
            padding: 0 1rem;
            color: rgb(24, 123, 216);
            text-transform: uppercase;
        }
    }

}



</style>