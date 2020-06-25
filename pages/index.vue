<template>


<div>
  
  <div>
  <p class="centre">logo</p>
  <section class="media">
    <div class="media-left">
    <figure class="image is-128x128">
   <img src="../assets/pattytup.jpg">
   </figure>
    </div>
  <div class="media-content">
     
  <h1 class="title centre">Pattytup</h1>
  <p class="centre">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Fugiat qui nemo soluta laboriosam.</p>
    
  </div>
</section>
</div>
<section>
  <br>
  <br>
  <h4 class="centre trait title is-4">Produits du moment</h4>
  <p class="centre">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
 
</section>
</div>


  
</template>

<script>
import Card from '~/components/Card'

export default {
  name: 'HomePage',

  components: {
    Card
  }
}
</script>


<style lang="css">
.centre{text-align: center;}
.trait:before, .trait:after { content:''; display:inline-block; vertical-align: middle; width: 2rem; height: 1px; background: #000 }
.trait:before { margin-right: .3rem }
.trait:after { margin-left: .3rem }
</style>