<script>
import axios from 'axios';
import PokemonCards from './PokemonCards.vue';
export default {
    components:{
        PokemonCards
    },
    data(){
        return{
            characterList:[]
        }
    },
    mounted(){
        axios.get('https://41tyokboji.execute-api.eu-central-1.amazonaws.com/dev/api/v1/pokemons?per=10').then((response) => {
            this.characterList = response.data.docs;
        })
    }
}
</script>

<template>
    <div class="container">
        <div class="row">
            <div class="col" v-for="(character,index) in characterList" :key="index">

                <PokemonCards :mycharacter="character" />

            </div>

        </div>
    </div>

</template>


<style lang="scss" scoped>
    

    .row{
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        align-items: center;

        .col{
        width: calc(100% / 5);
        }
    }

    
</style>