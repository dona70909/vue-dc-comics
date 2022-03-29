<template>
    <div  class="main-card">
        <img :src="card.thumb" alt="image">
        <p>{{card.series}}</p>
    </div>
</template>

<script>
export default {
    name:"CardMain",
    props:{
        card:Object,
    }
}
</script>

<style lang="scss" scoped>
.main-card{
    height: 250px;
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
</style>