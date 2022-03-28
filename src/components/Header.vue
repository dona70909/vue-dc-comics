<template>
    <div class="my-header-content d-flex">
        <div class="my-header-logo">
            <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <div class="my-header-nav">
            <ul class="d-flex my-link-list" >
                <li class="my-link-item" v-for="(link,index) in headerLinks" :key="index" >{{link.text}}</li>
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
                {text:"Comics",  url:"#"},
                {text:"Comics",  url:"#"},
                {text:"Comics",  url:"#"},
                {text:"Comics",  url:"#"},
                {text:"Comics",  url:"#"},
                {text:"Comics",  url:"#"}
            ]
        }

    }

}
</script>

<style lang="scss" scoped>

.my-header-content{
    justify-content: space-between;
    padding: 1rem;
    background-color:red;//solo per vederlo
}

.my-header-nav{

    line-height: 106.5px;
    .my-link-list{
        list-style-type:none;
        margin: 0;

        .my-link-item{
            padding: .5rem;
        }
    }
}



</style>