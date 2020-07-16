<template>
         <div class="is-hidden-desktop">
        <a href="/#anchor1" class="button retour is-hidden-desktop">^</a>
        <div class="barnav">
          <ul class="navicone">
            <li>
              <nuxt-link to="/">
              <i class="fa fa-home fa-2x" aria-hidden="true"></i>
              </nuxt-link>
            </li>
            <li>
               <nuxt-link to="/">
              <i class="fa fa-cutlery fa-2x" aria-hidden="true"></i>
              </nuxt-link>
            </li>
            <li>
               <nuxt-link to="/">
              <i class="fa fa-book fa-2x" aria-hidden="true"></i>
              </nuxt-link>
            </li>
            <li>
               <nuxt-link to="/">
              <i class="fa fa-address-card-o fa-2x" aria-hidden="true"></i>
              </nuxt-link>
            </li>
          </ul>
          </div>
        </div>
</template>


<style scoped>

body{
  /* background-color: lightblue; */
  height: 10000px;
  }
.barnav .navicone{

  background-color: white;
  position: fixed;
  overflow: hidden;
  bottom: 0;
  width: 100%;
  border-top: black solid 1px;
  list-style-type: none;

}

       .retour, .retour:visited{
         position: fixed;
         right: 4%;
         bottom:25.5vh;
         text-decoration: none;
       }

       .button, .button:visited{
         background-color: white;
         color: #6db6ca;
         font-size: 1.8em;

       }


       .button:hover{
         background-color: #6db6ca;
         color: white;
         text-decoration: none;
         }


.navicone{
  margin-left: 0;
    height:25vh;
    padding: 5px;
    display: flex;
    flex-direction : row;
    justify-content: space-around;


}

.fa {
    color: #6db6ca;
}



</style>
