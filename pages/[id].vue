<script setup>
    const route = useRoute();

    const { data: pokemon } = await useAsyncData(
        'pokemon',
        async () => await fetch('https://pokeapi.co/api/v2/pokemon/ditto'),
            { initialCache: false }
    );
    console.log(pokemon)
    
</script>
<template>
    
</template>