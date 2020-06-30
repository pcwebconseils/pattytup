<template>
    <nuxt-link   
        :to="id">
        <article class="post-preview">
            <div
                :style="{backgroundImage: 'url(' + thumbnailImage + ')'}"
                class="post-preview-thumbnail"></div>
                <div class="post-preview-content">
                <p>{{ categorie }}</p>
                <p>{{ nom }}</p>
                <p>{{ prix }}</p>
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
    background-position: center;
    background-size: cover;
    width:100% ;
    height: 10rem;
}

.post-preview-cotent{
    text-align: center;
    padding: 1rem;
}
</style>