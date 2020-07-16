<template>

<!-- carte produit avec lien vers single page -->
    <nuxt-link
        :to="id">
        <div class="post-preview  product-section">
            <div
                :style="{backgroundImage: 'url(' + thumbnailImage + ')'}"
                class="post-preview-thumbnail"></div>
                <div class="post-preview-content">
                  <span class="cat-product">{{ categorie }}</span>
                 <p class="name-product">{{ nom }}</p>
                 <span class="price-product">{{ prix }}</span>
            </div>
        </div>
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
        prix: {
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



/* css carte produit */





*{
    box-sizing:border box
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
    transition: 0.5s;
}

.name-product:hover {
    font-family: 'Montserrat', sans-serif;
    font-size: 17px;
    font-weight: bolder;
    margin-top: 1%;
    color: #6DB6CA;
    transition: 0.5s;
}


@media screen and (min-width: 35rem){
    .post-preview{
        width: 25rem;
        margin: 1rem;

    }
    
}


</style>