<script>

import AppHeader from './components/AppHeader.vue';
import PokemonList from './components/PokemonList.vue';


export default {
  components:{
    AppHeader,
    PokemonList
  }
}
</script>


<template>
  <div>
    <AppHeader/>
    
    <PokemonList/>
  </div>
</template>



<style lang="scss" scoped>

@use './styles/generals.scss' as *;

</style>