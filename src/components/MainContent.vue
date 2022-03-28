<template>
    <div class="my-main-wrapper">
        <div class="main-content padding">
            <h1> Content goes here</h1>
        </div>
    </div>
</template>

<script>
export default {

    name:"MainContentDc",

}
</script>

<style lang="scss" scoped>
.my-main-wrapper{
    width: 100%;
    height: 200px;
    padding:0;
    background-color: black;

    .main-content{    
        padding-top: 2rem;
        h1{
            color: white;
        }
    }
}
</style>