<template>
   <div class="container">
        <!-- Header -->
        <header class="head-col">
            <img src="../assets/fotolia.png" alt="Logo et image d'accueil" class="head-img">
            <div class="head-text">
                <h1 class="head-title">Pattytup</h1>
                <p class="head-desc">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi error aspernatur quisquam et enim
                    eaque voluptate
                    odit repellendus possimus a. Dolorum commodi earum cumque a corrupti suscipit, aut tenetur.
                </p>
            </div>
        </header>
        <!-- Section produits du moment -->
        <section>
            <h2 class="section-title">—— Produits du moment ——</h2>
            <p class="section-desc">Lorem ipsum dolor sit amet, consectetur.</p>
            <div class="columns product-section">
                <div class="column is-4-desktop is-12-mobile product-card">
                    <img src="../assets/product3.jpg" alt="Image du produit" class="img-product">
                    <span class="cat-product">Catégorie du produit</span>
                    <a href="#" class="name-product">Nom du produit</a>
                    <span class="price-product">15,00 €</span>
                </div>
                <div class="column is-4-desktop is-12-mobile product-card">
                    <img src="../assets/product3.jpg" alt="Image du produit" class="img-product">
                    <span class="cat-product">Catégorie du produit</span>
                    <a href="#" class="name-product">Nom du produit</a>
                    <span class="price-product">15,00 €</span>
                </div>
                <div class="column is-4-desktop is-12-mobile product-card">
                    <img src="../assets/product3.jpg" alt="Image du produit" class="img-product">
                    <span class="cat-product">Catégorie du produit</span>
                    <a href="#" class="name-product">Nom du produit</a>
                    <span class="price-product">15,00 €</span>
                </div>
            </div>
            <div>
           
            <nuxt-link to="./produit"><a class="btn-more">Découvrir plus</a></nuxt-link></div>
        </section>
        <!-- Section meilleures ventes -->
        <section>
            <h2 class="section-title">—— Meilleures ventes ——</h2>
            <p class="section-desc">Lorem ipsum dolor sit amet, consectetur.</p>
            <div class="columns product-section">
                <div class="column is-4-desktop is-12-mobile product-card">
                    <img src="../assets/product3.jpg" alt="Image du produit" class="img-product">
                    <span class="cat-product">Catégorie du produit</span>
                    <a href="#" class="name-product">Nom du produit</a>
                    <span class="price-product">15,00 €</span>
                </div>
                <div class="column is-4-desktop is-12-mobile product-card">
                    <img src="../assets/product3.jpg" alt="Image du produit" class="img-product">
                    <span class="cat-product">Catégorie du produit</span>
                    <a href="#" class="name-product">Nom du produit</a>
                    <span class="price-product">15,00 €</span>
                </div>
                <div class="column is-4-desktop is-12-mobile product-card">
                    <img src="../assets/product3.jpg" alt="Image du produit" class="img-product">
                    <span class="cat-product">Catégorie du produit</span>
                    <a href="#" class="name-product">Nom du produit</a>
                    <span class="price-product">15,00 €</span>
                </div>
            </div>
            <button class="btn-more">Découvrir plus</button>
        </section>
        <!-- Section denrières recettes -->
        <section>
            <h2 class="section-title">—— Dernières recettes ——</h2>
            <p class="section-desc">Lorem ipsum dolor sit amet, consectetur.</p>
            <div class="columns recipe-section">
                <div class="column is-6-desktop is-12-mobile recipe-card">
                    <img src="../assets/recipe.jpg" alt="Image de couverture pour la recette" class="img-recipe">
                    <span class="cat-recipe">Catégorie de la recette</span>
                    <a href="#" class="name-recipe">Nom de la recette</a>
                    <p class="description-recipe">
                        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Inventore sint natus amet, veniam
                        voluptate
                        ipsa voluptatem voluptates voluptatum suscipit, cumque error labore vel itaque laboriosam nobis
                        magni
                        excepturi eveniet libero.
                    </p>
                </div>
                <div class="column is-6x-desktop is-12-mobile recipe-card">
                    <img src="../assets/recipe.jpg" alt="Image de couverture pour la recette" class="img-recipe">
                    <span class="cat-recipe">Catégorie de la recette</span>
                    <a href="#" class="name-recipe">Nom de la recette</a>
                    <p class="description-recipe">
                        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Inventore sint natus amet, veniam
                        voluptate
                        ipsa voluptatem voluptates voluptatum suscipit, cumque error labore vel itaque laboriosam nobis
                        magni
                        excepturi eveniet libero.
                    </p>
                </div>
            </div>
            <button class="btn-more">Découvrir plus</button>
        </section>
        <!-- Section service Pattytup -->
        <section class="service">
            <h2 class="section-title">—— Service Pattytup ——</h2>
            <p class="section-desc">Lorem ipsum dolor sit amet, consectetur.</p>
            <div class="columns">
                <div class="column is-4-desktop is-12-mobile">
                    <img src="../assets/gift.svg" alt="Illustration" width="100">
                    <h3 class="serv-title">Produits de qualité</h3>
                    <p class="serv-desc">Lorem ipsum dolor sit amet, consectetur.</p>
                </div>
                <div class="column is-4-desktop is-12-mobile">
                    <img src="../assets/food-service.svg" alt="Illustration" width="100">
                    <h3 class="serv-title">Service après vente</h3>
                    <p class="serv-desc">Lorem ipsum dolor sit amet, consectetur.</p>
                </div>
                <div class="column is-4-desktop is-12-mobile">
                    <img src="../assets/return.svg" alt="Illustration" width="100">
                    <h3 class="serv-title">Retour sous 30 jours</h3>
                    <p class="serv-desc">Lorem ipsum dolor sit amet, consectetur.</p>
                </div>
            </div>
        </section>
    </div>
</template>

<script>

</script>

<style lang="css">

@media screen and (min-width: 1024px) {
  .container {margin-top:10rem;}
}

.container
{
 z-index: -1;}


/* HEADER */

header {
    display: flex;
    justify-content: center;
    align-items: center;
}

.head-img {
    width: 250px;
}

.head-text {
    width: 50%;
    margin-left: 4%;
}

.head-title {
    font-family: 'Montserrat', sans-serif;
    font-size: 40px;
    font-weight: bold;
    text-align: center;
}

.head-desc {
    text-align: justify;
    margin-top: 3%;
}


.centre {
  text-align: center;
}
.trait:before,
.trait:after {
  content: "";
  display: inline-block;
  vertical-align: middle;
  width: 2rem;
  height: 2px;
  background: #6db6ca;
}
.trait:before {
  margin-right: 0.3rem;
}
.trait:after {
  margin-left: 0.3rem;
}
.centre{
  margin-bottom: 2em;
}

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

/* Elément pour faire de l'espace*/

.root2{
  margin-top: 9%;
}

.root {
    margin-top: 4%;
    margin-bottom: 4%;
}

/* Produits */

section {
    justify-content: center;
    text-align: center;
}

.product-section {
    justify-content: center;
}


.product-card {
    display: flex;
    flex-direction: column;
    text-align: center;
}

.img-product {
    object-fit: cover !important;
    width: 70%;
    height: 55%;
    margin-left: auto;
    margin-right: auto;
}


.cat-product {
    font-family: 'Montserrat', sans-serif;
    font-size: 17px;
    font-weight: bold;
    color: #6DB6CA;
    margin-top: 1%;
}

.name-product, .price-product {
    font-family: 'Montserrat', sans-serif;
    font-size: 17px;
    font-weight: bolder;
    margin-top: 1%;
}

/*titre section*/

.section-title {
    font-family: 'Montserrat', sans-serif;
    font-size: 25px;
    font-weight: bold;
    text-align: center;
    margin-top: 5%;
}

.section-desc {
    font-family: 'Montserrat', sans-serif;
    font-size: 15px;
    font-style: italic;
    text-align: center;
    margin-top: 1%;
    margin-bottom: 5%;
}

@media only screen and (max-width: 430px) {
    .section-title {
        font-family: 'Montserrat', sans-serif;
        font-size: 20px;
        font-weight: bold;
        text-align: center;
        margin-top: 5%;
    }

    .section-desc {
        font-family: 'Montserrat', sans-serif;
        font-size: 13px;
        font-style: italic;
        text-align: center;
        margin-top: 1%;
        margin-bottom: 5%;
    }
  }

/* Recettes */

.recipe-section {
    justify-content: center;
}

.recipe-card {
    display: flex;
    flex-direction: column;
    margin-right: 1%;
}

.img-recipe {
    object-fit: cover !important;
    width: 100%;
    height: 50%;
    margin-left: auto;
    margin-right: auto;
}

.cat-recipe {
    font-family: 'Montserrat', sans-serif;
    font-size: 17px;
    font-weight: bold;
    color: #6DB6CA;
    margin-top: 1%;
}

.name-recipe {
    font-family: 'Montserrat', sans-serif;
    font-size: 17px;
    font-weight: bolder;
    margin-top: 1%;
}

.description-recipe {
    font-family: 'Montserrat', sans-serif;
    font-size: 17px;
    text-align: justify;
    margin-top: 1%;
}

/* Bouton */

.btn-more {
    font-family: 'Montserrat', sans-serif;
    font-size: 15px;
    font-weight: bolder;
    text-transform: uppercase;
    background-color: white;
    color: #6DB6CA;
    border: 1px solid #6DB6CA;
    border-radius: 10px;
    padding: 0.7%;
    padding-left: 3%;
    padding-right: 3%;
    cursor: pointer;
}

.btn-more:hover {
    font-family: 'Montserrat', sans-serif;
    font-size: 15px;
    font-weight: bolder;
    text-transform: uppercase;
    background-color: #6DB6CA;
    color: white;
    border: 1px solid #6DB6CA;
    border-radius: 10px;
    padding: 0.7%;
    padding-left: 3%;
    padding-right: 3%;
    cursor: pointer;
    transition: 0.5s;
}


/*service*/
@media screen and (max-width: 1024px){

.service{
  margin-bottom: 15rem;
}
}
</style>
