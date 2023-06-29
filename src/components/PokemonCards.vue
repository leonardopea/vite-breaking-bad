<script>
export default {
    props:{
        mycharacter:Object
    }
}
</script>

<template>
    <div>
        <img :src=" mycharacter.imageUrl ">
    </div>
</template>

<style lang="">
    
</style>