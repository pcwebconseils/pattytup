<template>
<main>
 <!-- barre de navigation desktop -->
  <div class="content is-hidden-desktop" id="anchor1"></div>
  <div class="is-hidden-touch">
          <nav class="columns navigation-d">
            <img class="column is-2 logo" src="../assets/logo.svg" alt="Logo">
               <ul class="column is-5 nav">
               <li class="navlink"><nuxt-link to="/"><a class="navhover" >Accueil</a></nuxt-link></li>
                <li class="navlink"><nuxt-link to="/produit"><a class="navhover" >Produit</a></nuxt-link></li>
              <li class="navlink"><nuxt-link to="/recette"><a class="navhover" >Recette</a></nuxt-link></li>
              <li class="navlink"><nuxt-link to="/contact"><a class="navhover" >Contact</a></nuxt-link></li>
               </ul>
              <form action="#" class="column is-2 search">
               <input class="searchbar" type="text" placeholder="Rechercher" name="search" size="7">
             <button class="search-i" type="submit"><i class="fa fa-search"></i></button>
           </form>
        </nav>
        </div>
        <!-- contenu -->
  
      
        <nuxt/>
   
      <!-- footer desktop -->

      <div class="is-hidden-touch">
        <footer>
            <p class="footer-cop">Copyright &copy; 2020 - PC Web Conseil</p>
            <p class="footer-text">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsa animi ullam tenetur. Maxime expedita, placeat
            iste
            saepe debitis, voluptatum libero harum magnam architecto odio sint cupiditate fugit amet, vitae itaque?
            Tempora dignissimos dolorum quam corporis quos, maxime cumque rerum laudantium modi veniam blanditiis quo
            nam,
            id amet! In voluptates natus delectus minima. Corporis maiores illo totam, molestiae eveniet explicabo
            magnam.
            Minima nihil delectus quae laboriosam mollitia natus velit repellat et in nobis aliquam alias, architecto,
            vitae
            accusantium modi optio fugiat cum recusandae minus ea sed ab ipsum, incidunt veritatis! Iure?
            Saepe, consequuntur voluptatum? Sed reiciendis enim aut. Saepe recusandae at reprehenderit vero doloremque
            rerum, deserunt eaque nihil quasi quo eveniet, voluptate blanditiis vel iste veritatis accusantium, velit
            quae.
            Provident, voluptatum.
            Officiis illo doloremque, cum ipsa beatae repellat veritatis voluptatibus dolorem sed quae odit aut, quo
            nulla
            officia molestias quis repellendus, voluptatum omnis autem nam non! Hic quaerat atque sequi deleniti!
        </p>
       </footer>
        </div>

  
      <!-- barre de navigation mobile/tablet -->
        
       <div class="is-hidden-desktop">
        <a href="/#anchor1" class="button retour is-hidden-desktop">^</a>
        <div class="barnav">
          <ul class="navicone">
            <li>
              <nuxt-link to="/">
              <i class="fa fa-home fa-2x" aria-hidden="true"></i>
              </nuxt-link>
            </li>
            <li>
               <nuxt-link to="/produit">
              <i class="fa fa-cutlery fa-2x" aria-hidden="true"></i>
              </nuxt-link>
            </li>
            <li>
               <nuxt-link to="/recette">
              <i class="fa fa-book fa-2x" aria-hidden="true"></i>
              </nuxt-link>
            </li>
            <li>
               <nuxt-link to="/contact">
              <i class="fa fa-address-card-o fa-2x" aria-hidden="true"></i>
              </nuxt-link>
            </li>
          </ul>
          </div>
        </div> 
  
  </main>
</template>


<script>




</script>

<style langue="css">

/* css barre de nav */


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
    height: 4rem;
    justify-content: center;
    align-items: center;
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

/*footer css*/

footer {
    background-color: #6DB6CA;
    color: white;
    margin-top: 3%;
    padding: 3%;
    box-shadow: 0px -4px 5px 0px rgba(0,0,0,0.75);
}

.footer-text {
    margin-top: 2%;
    text-align: justify;
}


/* css mobile/tablet */

.barnav .navicone{

  background-color: white;
  position: fixed;
  overflow: hidden;
  bottom: 0;
  width: 100%;
  border-top: black solid 1px;
  list-style-type: none;

}

       .retour, .retour:visited{
         position: fixed;
         right: 4%;
         bottom:25.5vh;
         text-decoration: none;
       }

       .button, .button:visited{
         background-color: white;
         color: #6db6ca;
         font-size: 1.8em;

       }


       .button:hover{
         background-color: #6db6ca;
         color: white;
         text-decoration: none;
         }


.navicone{
  margin-left: 0;
    height:25vh;
    padding: 5px;
    display: flex;
    flex-direction : row;
    justify-content: space-around;


}

.fa {
    color: #6db6ca;
}



</style>
