<template>

<div class="container">
    <section>
     <!-- Title -->
        <div class="product-section">
            <h1 class="section-title">—— Tous nos produits ——</h1>
            <p class="section-desc">Lorem ipsum dolor sit amet, consectetur.</p>
        </div>
            <!-- Filtrage des produits -->
        <div class="filter-box">
            <h2 class="filter-title">Filtrer</h2>
            <div class="columns is-12-mobile is-12-desktop filtre-col">
                <div class="column is-4-desktop is-12-mobile">
                    <h3 class="filter-cat">Par catégorie</h3>
                    <ul class="filter-option">
                        <li><input type="checkbox" name="catégorie" id="cat-id"><span class="checkmark"></span> Nom de la catégorie</li>
                        <li><input type="checkbox" name="catégorie" id="cat-id"><span class="checkmark"></span> Nom de la catégorie</li>
                        <li><input type="checkbox" name="catégorie" id="cat-id"><span class="checkmark"></span> Nom de la catégorie</li>
                        <li><input type="checkbox" name="catégorie" id="cat-id"><span class="checkmark"></span> Nom de la catégorie</li>
                        <li><input type="checkbox" name="catégorie" id="cat-id"><span class="checkmark"></span> Nom de la catégorie</li>
                    </ul>
                </div>
                <div class="column is-4-desktop is-12-mobile">
                    <h3 class="filter-cat">Par prix</h3>
                    <ul class="filter-option">
                        <li><input type="checkbox" name="prix" id="price-id"> 0€ à 10€</li>
                        <li><input type="checkbox" name="prix" id="price-id"> 10€ à 15€</li>
                        <li><input type="checkbox" name="prix" id="price-id"> 15€ à 25€</li>
                        <li><input type="checkbox" name="prix" id="price-id"> 25€ à 35€</li>
                        <li><input type="checkbox" name="prix" id="price-id"> 35€ et plus</li>
                    </ul>
                </div>
                <div class="column is-4-desktop is-12-mobile">
                    <h3 class="filter-cat">Par couleur</h3>
                    <ul class="filter-option">
                        <li><input type="checkbox" name="couleur" id="color-id-1" class="color-1"> Noir</li>
                        <li><input type="checkbox" name="couleur" id="color-id"> Rouge</li>
                        <li><input type="checkbox" name="couleur" id="color-id"> Bleu</li>
                        <li><input type="checkbox" name="couleur" id="color-id"> Jaune</li>
                        <li><input type="checkbox" name="couleur" id="color-id"> Orange</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <section class="container" id="posts">
        <PostPreview
            v-for="post in posts"
            :key="post.id"
            :categorie="post.categorie"
            :nom="post.nom"
            :prix="post.prix"
            :thumbnailImage="post.thumbnailUrl"
            :id="post.id" />
  </section>
</div>
</template>

<script>
// importe du component PostPreview
    import PostPreview from "@/components/Posts/PostPreview";
    export default {
        components: {
            PostPreview
        },
        asyncData(context){
            return context.app.$storyapi.get('cdn/stories',
            {version: 'draft',
            starts_with:'produit/'
            }).then(res => {
                console.log(res);
                // array de data recuperer sur storyblok
                return {posts: res.data.stories.map(bp =>{
                    return{
                        id:bp.slug,
                        categorie: bp.content.categorie_produit,
                        nom: bp.content.nom_produit,
                        prix: bp.content.prix,
                        thumbnailUrl: bp.content.image_produit.filename

                    };

                })
            };
            });
        }
  
    };
</script>


<style scoped>
/* css produit et filtre */
.container{
    
    padding-top: 0rem;
}

.section-title {
    font-family: 'Montserrat', sans-serif;
    font-size: 25px;
    font-weight: bold;
    text-align: center;
  
}

.section-desc {
    font-family: 'Montserrat', sans-serif;
    font-size: 15px;
    font-style: italic;
    text-align: center;
    margin-top: 1%;
    margin-bottom: 5%;
}



#posts{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
   
}

.product-section {
    justify-content: center;
    text-align: center;
}

.product-section > .section-title {
    font-family: 'Montserrat', sans-serif;
    font-size: 25px;
    font-weight: bold;
    text-align: center;
}

.filter-box {
    border: 1px solid #ccc;
    border-radius: 4px;
    box-shadow: 0 0 6px 0 rgba(0,0,0,0.1);
    background-color: #ffffff;
    margin-bottom: 5%;
    padding: 2%;
}

.filter-title {
    font-family: 'Montserrat', sans-serif;
    font-size: 19px;
    font-weight: bold;
    text-align: center;
}

.filter-cat {
    font-family: 'Montserrat', sans-serif;
    font-size: 17px;
    font-weight: bold;
    text-align: center;
}

.filter-option {
    font-family: 'Montserrat', sans-serif;
    font-size: 15px;
    text-align: center;
    margin-top: 3%;
}

.product-section {
    justify-content: center;
}


@media screen and ( min-width: 1024px){
    /* .container{padding-top: 3.5rem;} */
    #posts{
        flex-direction: row;
    };
}

</style>