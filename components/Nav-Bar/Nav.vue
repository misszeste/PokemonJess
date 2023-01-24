
  <style>
  *
    {
      box-sizing: border-box;
      font-family: Arial, Helvetica, sans-serif;
    }

    body {
      margin: 0;
      font-family: Arial, Helvetica, sans-serif;
    }

    /* Style the top navigation bar */
    .topnav {
      overflow: hidden;
      background-color: #333;
    }

    /* Style the topnav links */
    .topnav a {
      float: left;
      display: block;
      color: #f2f2f2;
      text-align: center;
      padding: 14px 16px;
      text-decoration: none;
    }

    /* Change color on hover */
    .topnav a:hover {
      background-color: rgb(231, 226, 226);
      color: rgb(109, 36, 36);
    }
</style>

<template>
    <head>
        <title>Démo E14</title>
    </head> 
    <div class="topnav">    
      <!-- Utilisation de NuxtLink -->
      <NuxtLink to="/">Accueil</NuxtLink>    
      <!-- hidden en mode connecter -->
      <NuxtLink to="/login">S'inscrire</NuxtLink>    
          <!-- hidden en mode deconnecter -->  
      <NuxtLink to="/connecter/liste" >Liste de Pokémon</NuxtLink>      
      <NuxtLink to="/connecter/deconnecter">Se deconnecter</NuxtLink>      
    </div> 
    
</template>