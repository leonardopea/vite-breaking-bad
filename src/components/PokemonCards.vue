<script>
export default {
    props:{
        mycharacter:Object
    }
}
</script>

<template>
    <div class="container">
        <img :src=" mycharacter.imageUrl ">
        <h1>{{ mycharacter.number }}</h1>
        <h2>{{ mycharacter.name }}</h2>
        <h3>{{ mycharacter.type1 }}</h3>
    </div>
</template>

<style lang="scss" scoped>
    img{
        width: 150px;
        height: 150px;
        border-radius: 50%;
        padding-top: 10px;
        
    }

    .container{
        background-color: rgb(63, 147, 147);
        height: 350px;
        border-radius: 20px;
        margin: 20px;
        text-align: center;
        
    }
</style>