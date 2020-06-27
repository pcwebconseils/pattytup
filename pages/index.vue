<template>

  <main class="">
    <div class="root2 is-hidden-touch"></div>
    <div>
      <p class="centre is-hidden-desktop">logo-image</p>
      <section class="media">
        <div class="media-left">
          <figure class="image is-128x128 patty"></figure>
        </div>
      </section>
    </div>
  <div>
    <div>
      <p class="centre">logo-image</p>
      <section class="media">
        <div class="media-left">
          <figure class="image is-128x128">

            <img src="../assets/pattytup.jpg" />
          </figure>
        </div>
        <div class="media-content">
          <h1 class="title centre">Pattytup <br> Tupperware et recettes</h1>
          <h2 class="centre">
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Fugiat qui
            nemo soluta laboriosam.
          </h2>
        </div>
      </section>
    </div>
    <section>
      <h3 class="centre trait title is-4 ">Recettes de la semaine</h3>
      <p class="centre">

        Lorem Lorem ipsum dolor sit amet consectetur adipisicing elit.
      </p>

    <section>
        <div class="columns product-section">
            <div class="column is-3-desktop is-12-mobile product-card">
                <img src="../assets/product.jpg" alt="Image du produit" class="img-product">
                <span class="cat-product">Catégorie du produit</span>
                <a href="#" class="name-product patty">Nom du produit</a>
                <span class="price-product">15,00 €</span>
            </div>
            <div class="column is-3-desktop is-12-mobile product-card">
                <img src="../assets/product2.jpg" alt="Image du produit" class="img-product">
                <span class="cat-product">Catégorie du produit</span>
                <a href="#" class="name-product patty">Nom du produit</a>
                <span class="price-product">15,00 €</span>
            </div>
            <div class="column is-3-desktop is-12-mobile product-card">
                <img src="../assets/product3.jpg" alt="Image du produit" class="img-product">
                <span class="cat-product">Catégorie du produit</span>
                <a href="#" class="name-product patty">Nom du produit</a>
                <span class="price-product">15,00 €</span>
            </div>
        </div>
        <button class="btn-more">Découvrir plus</button>
        <div class="root"></div>
    </section>

        Lorem ipsum dolor sit amet consectetur adipisicing elit.

    </section>
    <section>
      <h3 class="centre trait title is-4">Produits du moment</h3>
      <p class="centre">
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
      </p>


      <section>
        <div class="columns recipe-section">
            <div class="column is-4 recipe-card">
                <img src="../assets/recipe.jpg" alt="Image de couverture pour la recette" class="img-recipe">
                <span class="cat-recipe">Catégorie de la recette</span>
                <a href="#" class="name-recipe patty">Nom de la recette</a>
                <p class="description-recipe">
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit. Inventore sint natus amet, veniam voluptate
                    ipsa voluptatem voluptates voluptatum suscipit, cumque error labore vel itaque laboriosam nobis magni
                    excepturi eveniet libero.
                </p>
            </div>
            <div class="column is-4 recipe-card">
                <img src="../assets/recipe.jpg" alt="Image de couverture pour la recette" class="img-recipe">
                <span class="cat-recipe">Catégorie de la recette</span>
                <a href="#" class="name-recipe patty">Nom de la recette</a>
                <p class="description-recipe">
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit. Inventore sint natus amet, veniam voluptate
                    ipsa voluptatem voluptates voluptatum suscipit, cumque error labore vel itaque laboriosam nobis magni
                    excepturi eveniet libero.
                </p>
            </div>
        </div>
        <button class="btn-more">Découvrir plus</button>
    </section>

    </section>
  </div>
  </main>
</template>

<script>
import Card from "~/components/Card";

export default {
  name: "HomePage",

  components: {
    Card
  }
};
</script>

<style lang="css">


.patty{
  z-index: -1;
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
    margin-top: 5%;
    margin-bottom: 5%;
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
    margin-top: 2em;
}

.description-recipe {
    font-family: 'Montserrat', sans-serif;
    font-size: 17px;
    text-align: justify;
    margin: 2em;
  
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


</style>
