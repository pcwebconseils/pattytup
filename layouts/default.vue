<template>
      <div >

        <nuxt />
        <div class="navbar">
          <ul>
            <li>
              <nuxt-link to="/">
              <i class="fa fa-home" aria-hidden="true"></i>
              </nuxt-link>
            </li>
            <li>
               <nuxt-link to="/">
              <i class="fa fa-cutlery" aria-hidden="true"></i>
              </nuxt-link>
            </li>
            <li>
               <nuxt-link to="/">
              <i class="fa fa-book" aria-hidden="true"></i>
              </nuxt-link>
            </li>
            <li>
               <nuxt-link to="/">
              <i class="fa fa-address-card-o" aria-hidden="true"></i>
              </nuxt-link>
            </li>
          </ul>
          </div>
      </div>
</template>

<style langue="css">

.navbar ul{
 overflow: hidden;
  position: fixed;
  bottom: 0;
  width: 100%;
  border-top: black solid 1px;

}

ul{

    padding: 5px;
    display: flex;
    flex-direction : row;
    justify-content: space-around;

};

i {
    color: black;
}
.fa {
    color: black;
}

</style>
