<template>

<main>
 <!-- barre de navigation desktop -->
  <div class="content" id="anchor1"></div>
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

  <div class="content" id="anchor1">


      <!-- contenu -->
        <nuxt />

      <!-- footer desktop -->



      <!-- barre de navigation mobile/tablet -->
        <div class="is-hidden-desktop">
        <a href="/#anchor1" class="button retour is-hidden-desktop">^</a>


        <a class="retour"><nuxt-link :to="{path: '/', hash: '#anchor1'}" class="button">^</nuxt-link></a>

        <div class="barnav">
          <ul class="navicone">
            <li>
              <nuxt-link to="/">
              <i class="fa fa-home fa-2x" aria-hidden="true"></i>
              </nuxt-link>
            </li>
            <li>
               <nuxt-link to="/">
              <i class="fa fa-cutlery fa-2x" aria-hidden="true"></i>
              </nuxt-link>
            </li>
            <li>
               <nuxt-link to="/">
              <i class="fa fa-book fa-2x" aria-hidden="true"></i>
              </nuxt-link>
            </li>
            <li>
               <nuxt-link to="/">
              <i class="fa fa-address-card-o fa-2x" aria-hidden="true"></i>
              </nuxt-link>
            </li>
          </ul>
          </div>

        </div>
  </div>

<footer>
  <nav class="is-hidden-touch bas">
    <ul>
      <li>Mentions légales</li>
      <li>Mentions légales</li>
    </ul>
  </nav>
</footer>
 </main>

</template>

<style langue="css">



/* Desktop format */
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
  width: 75%;
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


/* css mobile/tablet */


body{
  background-color: rgba(190, 236, 252, 0.144); 
  /*height: 100vh;*/
  }
.barnav .navicone{

  background-color: white;
  position: fixed;
  overflow: hidden;
  bottom: 0;
  width: 100%;
  border-top: #6db6ca solid 2px;
  list-style-type: none;
  margin: 0;

}

       .retour, .retour:visited{
         position: fixed;
          right: 5%;
         bottom:18vh;
         text-decoration: none;
       }

       .button, .button:visited{
         background-color: rgba(52, 146, 223, 0.281);

         color: rgba(109, 182, 202, 0.459);
         font-size: 1.8em;


         color: rgba(173, 216, 230, 0.411);
         font-size: 1.8em;



       }


       .button:hover{

         background-color: #6db6ca;

         background-color: lightblue;

         color: white;
         text-decoration: none;
         }


.navicone{
    height:15vh;
    padding: 5px;
    display: flex;
    flex-direction : row;
    justify-content: space-around;
}

.fa {
    color: #6db6ca;
}
.bas ul{
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  background-color: #6DB6CA;
  width: 100%;
  height: 5vh;
}
.bas ul li{
  height: 80%;
  color: aliceblue;
}


</style>
