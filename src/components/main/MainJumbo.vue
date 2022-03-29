<template>
    <div class="my-jumbo">
        <img :src="require('@/assets/img/jumbotron.jpg')" alt="jumbo">
    </div>
</template>

<script>
export default {
    name:"MainJumbo",

}
</script>

<style lang="scss" scoped>
    .my-jumbo{
        height: 400px;

        img{
            height: 100%;
            width:100%;
            object-fit: cover;
            object-position: 50% 10%;
        }
    }
</style>