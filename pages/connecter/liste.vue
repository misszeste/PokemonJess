<script setup>
    const pokemonsRequest = await fetch(`
        https://pokeapi.co/api/v2/pokemon?limit=100`
    );
    const pokemonsList = await pokemonsRequest.json();

    const list = await pokemonsList.results.map(async (pokemon) => {
        const pokemonTemp = await fetch(pokemon.url);
        return pokemonTemp.json();
    });

    let pokemonWithDetails = [];

    Promise.all(list).then((values) => {
        pokemonWithDetails.push(values);
    });
    console.log(pokemonWithDetails)
</script>
<template>
    <ul>
        <li v-for= "pokemon in pokemonWithDetails[0]" :key="pokemon.name" :pokemon="pokemon">
            <a>
                <img :src="pokemon.sprites.front_default" alt="" srcset="">
                {{ pokemon.name}}
            </a>
        </li>
    </ul>
</template>

