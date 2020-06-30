<template>
     <div class="container">
        <div class="recipe-section">
            <h1 class="section-title">—— Découvrez nos recettes ——</h1>
        </div>

        <section>
            <h2 class="section-title">—— Nos entrées ——</h2>
            <p class="section-desc">Lorem ipsum dolor sit amet, consectetur.</p>
            <div class="columns product-section">
                <div class="column is-4-desktop is-12-mobile recipe-card">
                    <img src="assets/plat.jpg" alt="Image du produit" class="img-cat">
                    <a href="#" class="name-cat-recipe">Catégorie de recette</a>
                </div>
                <div class="column is-4-desktop is-12-mobile recipe-card">
                    <img src="assets/plat.jpg" alt="Image du produit" class="img-cat">
                    <a href="#" class="name-cat-recipe">Catégorie de recette</a>
                </div>
                <div class="column is-4-desktop is-12-mobile recipe-card">
                    <img src="assets\plat.jpg" alt="Image du produit" class="img-cat">
                    <a href="#" class="name-cat-recipe">Catégorie de recette</a>
                </div>
            </div>
        </section>

        <section>
            <h2 class="section-title">—— Nos plats ——</h2>
            <p class="section-desc">Lorem ipsum dolor sit amet, consectetur.</p>
            <div class="columns product-section">
                <div class="column is-4-desktop is-12-mobile recipe-card">
                    <img src="assets\plat.jpg" alt="Image du produit" class="img-cat">
                    <a href="#" class="name-cat-recipe">Catégorie de recette</a>
                </div>
                <div class="column is-4-desktop is-12-mobile recipe-card">
                    <img src="assets\plat.jpg" alt="Image du produit" class="img-cat">
                    <a href="#" class="name-cat-recipe">Catégorie de recette</a>
                </div>
                <div class="column is-4-desktop is-12-mobile recipe-card">
                    <img src="assets\plat.jpg" alt="Image du produit" class="img-cat">
                    <a href="#" class="name-cat-recipe">Catégorie de recette</a>
                </div>
            </div>
        </section>

        <section class="dessert">
            <h2 class="section-title">—— Nos desserts ——</h2>
            <p class="section-desc">Lorem ipsum dolor sit amet, consectetur.</p>
            <div class="columns product-section">
                <div class="column is-4-desktop is-12-mobile recipe-card">
                    <img src="assets\plat.jpg" alt="Image du produit" class="img-cat">
                    <a href="#" class="name-cat-recipe">Catégorie de recette</a>
                </div>
                <div class="column is-4-desktop is-12-mobile recipe-card">
                    <img src="assets/plat.jpg" alt="Image du produit" class="img-cat">
                    <a href="#" class="name-cat-recipe">Catégorie de recette</a>
                </div>
                <div class="column is-4-desktop is-12-mobile recipe-card">
                    <img src="assets/plat.jpg" alt="Image du produit" class="img-cat">
                    <a href="#" class="name-cat-recipe">Catégorie de recette</a>
                </div>
            </div>
        </section>
    </div>
</template>

<style scoped>
/* Recettes */

.recipe-section {
    justify-content: center;
}

.recipe-card {
    display: flex;
    flex-direction: column;
    margin-right: 1%;
    justify-content: center;
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

@media only screen and (max-width: 770px) {
    .recipe-card {
        display: flex;
        flex-direction: column;
        padding: 6%;
        justify-content: center;
    }
  }

  .recipe-section {
    justify-content: center;
    text-align: center;
}

.recipe-section > .section-title {
    font-family: 'Montserrat', sans-serif;
    font-size: 25px;
    font-weight: bold;
    text-align: center;
}

.recipe-card {
    display: flex;
    flex-direction: column;
    text-align: center;
}

.img-cat {
    object-fit: cover !important;
    width: 100%;
    margin-left: auto;
    margin-right: auto;
}

.name-cat-recipe {
    font-family: 'Montserrat', sans-serif;
    font-size: 17px;
    font-weight: bolder;
    margin-top: 1%;
    transition: 0.3s;
}

.name-cat-recipe:hover {
    color: #6DB6CA;
    font-family: 'Montserrat', sans-serif;
    font-size: 17px;
    font-weight: bolder;
    margin-top: 1%;
    transition: 0.3s;
}

@media only screen and (max-width: 770px) {
    .img-cat {
        object-fit: cover !important;
        width: 70%;
        max-height: 400px;
        height: auto;
    }
  }

@media only screen and (max-width: 500px) {
    .img-cat {
        object-fit: cover !important;
        width: 70%;
        max-height: 270px;
        height: auto;
    }
  }

@media only screen and (max-width: 375px) {
    .img-cat {
        object-fit: cover !important;
        width: 70%;
        max-height: 200px;
        height: auto;
    }
  }


@media screen and (max-width: 1024px){

.dessert{
  margin-bottom: 13rem;
}
}

</style>