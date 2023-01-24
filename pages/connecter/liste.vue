<script setup>
    // déclaration variable
    const pokemonRequest = await fetch('https://pokeapi.co/api/v2/pokemon?limit=12')
    const pokemonRequestImage = await fetch('https://pokeapi.co/api/v2/pokemon/')
    const pokemonList = await pokemonRequest.json()   
    const pokemonListImage = await pokemonRequestImage.json() 
</script>

<template>         
    <!-- appel component Card -->          
    <Card v-for="pokemon in pokemonList.results" :key="pokemon.name" :pokemon="pokemon">
        {{ pokemon.name}}        
    </Card> 
    <nav aria-label="Page navigation example" >
        <div class="pagination">
            <div class="page-item"><a class="page-link" href="#">Previous</a></div>
            <div class="page-item"><a class="page-link" href="#">1</a></div>
            <div class="page-item"><a class="page-link" href="#">2</a></div>          
            <div class="page-item"><a class="page-link" href="#">Next</a></div>
        </div>
    </nav>       
</template>

