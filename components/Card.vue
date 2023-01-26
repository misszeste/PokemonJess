<script setup>
    const props = defineProps({
        pokemon: Object,
    });
    const { pokemon } = props;
 
console.log(pokemon)
    

    // const list = document.getElementById("list");
    // const getPokemons = async () =>{
    //     const poke = await fetch("https://pokeapi.co/api/v2/pokemon")
    //     return await poke.json();
    //     }

    //     const getSinglePokemon = async (url) =>{
    //     const poke = await fetch(url)
    //     return await poke.json();
    //     }


    // const pokemons =  getPokemons();
    // pokemons.then((res)=> {
    //     res.results.forEach(pokemon => {
    //         const info =  getSinglePokemon(pokemon.url).then((res) =>{
    //         const li = document.createElement("li");
    //         const img = document.createElement("img")
       
    //         img.src = res.sprites.front_default
    //         li.textContent = pokemon.name;            
    //         li.appendChild(img)
    //         list.appendChild(li)
    //         })

    //     });
    // })


</script>



<template > 
   <li>
    {{ pokemon.name }}
   </li>
</template>

<style scoped>

    li{
        text-align: center;
        text-transform: capitalize;
        display: flex;
        font-size: 25px;
        font-family: sans-serif;
        flex-direction: column;
        padding: 50px;
        border: 1px solid black;
        border-radius: 25px;
    }

    .card-header{
        background-color:blueviolet ;
       
    }

    .card-text{
        background-color:blueviolet ;
    }
    .card-img-top{
        background-color:blueviolet ;
    }
    .card{
      
        width: 33%;
    }
</style>