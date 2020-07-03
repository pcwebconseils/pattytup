<template>



<!-- carte recette avec lien vers single page -->
    <nuxt-link   
        :to="id">
        <article class="post-preview">
            <div
                :style="{backgroundImage: 'url(' + thumbnailImage + ')'}"
                class="post-preview-thumbnail"></div>
                <div class="post-preview-content">
                 <h1 class="cat-product">{{ categorie }}</h1>
                  <p class="name-product">{{ nom }}</p>
            </div>
        </article>
    </nuxt-link>
</template>

<script>
export default {
    props:{
        categorie: {
            type: String,
            required: true
        },
        nom: {
            type: String,
            required: true
        },
        thumbnailImage: {
            type: String,
            required: true
        },
        id: {
            type: String,
            required: true
        }
    }
    
};
</script>

<style scoped>

/* css carte recette */


*{
    box-sizing:border box
}

a{
    text-decoration: none;
    color: black;
}

.post-preview{
    border-radius: 3px;
    border: black solid 1px;
    box-shadow: 1px 1px 5px 1px rgba(0,0,0,0.5);
    width: 90%;
    margin: auto;
    height: 20rem;
}

.post-preview-thumbnail{
    width: 100%;
    height: 100%;
    background-position: center;
    background-size: cover;
    width:100% ;
    height: 10rem;
}

.post-preview-cotent{
    text-align: center;
    padding: 1rem;
}


a{
    text-decoration: none;
    color: black;
}

.post-preview{
    
    border-radius: 3px;
    box-shadow: 1px 1px 5px 1px rgba(0,0,0,0.5);
    width:90%;
    margin: auto;
    height: 20rem;
   
    
}

.post-preview-thumbnail{
  
    background-position: center;
    background-size: cover;
    width:100% ;
    height: 10rem;
}

.post-preview-cotent{
    text-align: center;
    padding: 1rem;
}


@media screen and (min-width: 35rem){
    .post-preview{
        width: 25rem;
        margin: 1rem;

    }
    
}
</style>