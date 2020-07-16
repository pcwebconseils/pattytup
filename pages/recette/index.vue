<template>

<div class="container">
    <section>

    
 
        <div class="recipe-section">
            <h1 class="section-title">—— Découvrez nos recettes ——</h1>
        </div>

    </section>

    <section class="container" id="posts">
        <RecettePreview
            v-for="post in posts"
            :key="post.id"
            :categorie="post.categorie"
            :nom="post.nom"
            :thumbnailImage="post.thumbnailUrl"
            :id="post.id" />
  </section>
</div>
</template>

<script>
// importe du component RecettePreview
    import RecettePreview from "@/components/Recette/RecettePreview";
    export default {
        components: {
            RecettePreview
        },
        asyncData(context){
            return context.app.$storyapi.get('cdn/stories',
            {version: 'draft',
            starts_with:'recette/'
            }).then(res => {
                console.log(res);
                 // array de data recuperer sur storyblok
                return {posts: res.data.stories.map(bp =>{
                    return{
                        id:bp.slug,
                        categorie: bp.content.categorie_recette,
                        nom: bp.content.nom_recette,
                        thumbnailUrl: bp.content.photo_recette.filename

                    };

                })
            };
            });
        }

    };
</script>


<style scoped>

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

@media screen and (min-width: 1024px) {
  .container {margin-top:150px;}
}


@media screen and ( min-width: 1024px){
    /* .container{padding-top: 3.5rem;} */
    #posts{
        flex-direction: row;
    };
}

@media screen and (max-width: 1024px) {
  .container {margin-bottom:15rem;}
}


</style>