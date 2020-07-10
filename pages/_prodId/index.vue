<template>
    <!-- recuperation id pour single page -->

    <div class="container" id="posts">

        <div class="info-page">
            <div class="column is-6-desktop is-12-mobile">
                <div class="info">
                    <div
                        class="post-thumbnail infop-img"
                        :style="{backgroundImage: 'url(' + image +')'}"></div>
                    <h3 class="infop-name">{{ title}}</h3>
                    <p class="infop-price">
                        {{ prix }}</p>
                    <p class="infop-desc is-6-desktop is-12-mobile">
                        {{ description }}
                    </p>

                </div>

            </div>
        </div>

    </div>

</template>

<script>
    export default {
        asyncData(context) {
            return context
                .app
                .$storyapi
                .get('cdn/stories/produit/' + context.params.prodId, {version: 'draft'})
                .then(res => {

                    return {
                        image: res.data.story.content.photo_recette.filename,
                        title: res.data.story.content.nom_produit,
                        prix: res.data.story.content.prix,
                        description: res.data.story.content.description_produit,
                        categorie: res.data.story.content.categorie_produit
                    };

                });
        }
    };
</script>

<style scoped="scoped">

  
/* Page d'un produit */

.info-page {
    display: flex;
    justify-content: center;
}

.infop-img {
    object-fit: cover !important;
    width: 100%;
    height: 55%;
    margin-left: auto;
    margin-right: auto;
}


.cat-product {
    font-family: 'Montserrat', sans-serif;
    font-size: 20px;
    font-weight: bold;
    color: #6DB6CA;
    margin-top: 1%;
}

.infop-name, .infop-price {
    font-family: 'Montserrat', sans-serif;
    font-size: 20px;
    font-weight: bolder;
    margin-top: 1%;
    text-align: center;
}

.infop-name {
    transition: 0.5s;
}

.infop-name:hover {
    color: #6DB6CA;
    transition: 0.5s;
}

.infop-desc {
    text-align: justify;
}

</style>