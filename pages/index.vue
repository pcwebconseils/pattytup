<template>
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
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
      </p>
    </section>
    <section>
      <h3 class="centre trait title is-4">Produits du moment</h3>
      <p class="centre">
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
      </p>
    </section>
  </div>
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
</style>
