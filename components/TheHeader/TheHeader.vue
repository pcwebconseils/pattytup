
<template>



<div class="is-hidden-touch">
          <nav class="columns navigation-d">
            <img class="column is-2 logo" src="../assets/logo.svg" alt="Logo">
               <ul class="column is-5 nav">
               <li class="navlink"><a class="navhover" href="#">Accueil</a></li>
                <li class="navlink"><a class="navhover" href="#">Produits</a></li>
               <li class="navlink"><a class="navhover" href="#">Recettes</a></li>
               <li class="navlink"><a class="navhover" href="#">Contact</a></li>
               </ul>
              <form action="#" class="column is-2 search">
               <input class="searchbar" type="text" placeholder="Rechercher" name="search" size="7">
             <button class="search-i" type="submit"><i class="fa fa-search"></i></button>
           </form>
        </nav>
        </div>

</template>

<style langue="css">
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

a, li {
    position: relative;
    text-decoration: none;
    list-style: none;
    color: inherit;
}

a:hover {
    color: inherit;
}



.navigation-d {
    position: fixed;
    top: 0;
    left: 0;
    width: 105%;
    background-color: #6DB6CA;
    justify-content: center;
    align-items: center !important;
    padding-top: 2%;
    padding-bottom: 2%;
    box-shadow: 0px 4px 5px 0px rgba(0,0,0,0.75);
}

.nav {
    justify-content: center;
    display: flex;
}

.navlink {
    font-family: 'Poppins', sans-serif;
    font-size: 17px;
    color: white;
    text-transform: uppercase;
    margin-right: 4%;
}

.navhover::after {
    content: '';
    position: absolute;
    bottom: 0;
    left: 0;
    width: 0;
    border-bottom: 3px solid white;
    transition: 0.7s;
}

.navhover:hover::after{
    width: 100%;
}

.logo {
    width: 12% !important;
    text-align: center;
}

.search {
    text-align: center;
}

.searchbar {
    background-color: #86BFD1;
    color: white;
    font-family: 'Poppins', sans-serif;
    font-size: 15px;
    border: none;
    border-top-left-radius: 10px;
    border-bottom-left-radius: 10px;
    padding: 2%;
    padding-left: 5%;
    margin-right: -1%;
}

::placeholder {
    color: white;
}

.search-i {
    background-color: #86BFD1;
    color: white;
    font-family: 'Poppins', sans-serif;
    font-size: 15px;
    border: none;
    cursor: pointer;
    border-top-right-radius: 10px;
    border-bottom-right-radius: 10px;
    padding: 2%;
    padding-right: 5%;
    margin-left: -1%;
}

</style>