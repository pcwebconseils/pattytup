<template>
 <!-- template single page d'une recette -->
   
            <div class="container"  id="posts" v-editable="blok">
        <div class="info-recipe">
            <div class="info">
              <div class="post-thumbnail info-img-recipe" :style="{backgroundImage: 'url(' + image +')'}"></div>
                <h1 class="info-title">{{ title}}</h1>
            </div>
            <div class="columns info-head">
                <div class="column is-2-desktop info-card">
                    <img src="../../assets/four.png" alt="icone" class="info-img">
                     <p> {{ cuisson }}</p>
                </div>
                <div class="column is-2-desktop info-card">
                    <img src="../../assets/mixer.png" alt="icone" class="info-img">
                   <p> {{ preparation }}</p>
                </div>
                <div class="column is-2-desktop info-card">
                    <img src="../../assets/toque.png" alt="icone" class="info-img">
                    <p> {{ difficulte }}</p>
                </div>
            </div>
            <div class="columns info-main">
                <div class="column is-4-desktop info-ingr">
                  <p> {{ ingredient }}</p>
                </div>
                <div class="column is-5-desktop info-step">
                    <p> {{ etape }}</p>
                </div>
            </div>
        </div>
    </div>

</template>

<script>
export default {
  asyncData(context){
      return context.app.$storyapi.get('cdn/stories/recette/' + context.params.postId, {
          version: 'draft'
      }).then(res => {
       
        return {
        blok: res.data.story.content,
        image: res.data.story.content.photo_recette.filename,
        title: res.data.story.content.nom_recette,
        etape: res.data.story.content.liste_etape,
        cuisson: res.data.story.content.cuisson,
        difficulte:res.data.story.content.difficulte,
        preparation: res.data.story.content.preparation,
        ingredient:res.data.story.content.liste_ingredient,
        categorie:res.data.story.content.categorie_recette,

      };

      });
  }  
};
</script>


<style scoped>




.post-thumbnail {
 
 width:665px;
  height: 271px;
  background-size: cover;
  margin-left: auto;
  margin-right: auto;
  background-position: center;
}
.info {
    text-align: center;
}

.info > .info-title {
    font-family: 'Montserrat', sans-serif;
    font-size: 20px;
    font-weight: bolder;
    margin-top: 2%;
    margin-bottom: 2%;
    text-align: center;
    transition: 0.5s;
}

.info > .info-title:hover {
    font-family: 'Montserrat', sans-serif;
    font-size: 20px;
    font-weight: bolder;
    margin-top: 2%;
    margin-bottom: 2%;
    text-align: center;
    color: #6DB6CA;
    transition: 0.5s;
}

.info-head {
    justify-content: center;
}

.info-card {
    text-align: center;
}

.info-main {
    justify-content: center;
}

.info-ingr-title, .info-step-title {
    font-family: 'Montserrat', sans-serif;
    font-size: 17px;
    font-weight: bolder;
    margin-top: 4%;
    margin-bottom: 7%;
    text-align: center;
}

.info-ingr > ul > li {
    margin-top: 2%;
    text-align: center;
}

.info-step > p {
    text-align: justify;
}

@media only screen and (max-width: 1024px) {
    .info-step > p {
        text-align: justify;
        padding: 5%;
    }
}

@media screen and (max-width: 1024px) {
  .container {margin-bottom:14rem;}
}


</style>