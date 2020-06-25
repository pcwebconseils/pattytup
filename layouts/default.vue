<template>
  <div class="content">
    <nuxt />

    <div class="barnav">
      <ul>
        <li>
          <nuxt-link to="/">
            <i class="fa fa-home fa-3x" aria-hidden="true"></i>
          </nuxt-link>
        </li>
        <li>
          <nuxt-link to="/">
            <i class="fa fa-cutlery fa-3x fa-border" aria-hidden="true"></i>
          </nuxt-link>
        </li>
        <li>
          <nuxt-link to="/">
            <i class="fa fa-book fa-3x" aria-hidden="true"></i>
          </nuxt-link>
        </li>
        <li>
          <nuxt-link to="/">
            <i class="fa fa-address-card-o fa-3x" aria-hidden="true"></i>
          </nuxt-link>
        </li>
      </ul>
    </div>
  </div>
</template>

<style langue="css">
body{background-color: lightblue;}
.barnav ul {
  background-color: white;
  position: fixed;
  overflow: hidden;
  bottom: 0;
  width: 100%;
  border-top: black solid 1px;
  list-style-type: none;
}

ul {
  margin-left: 0;
  height: 25vh;
  padding: 5px;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
}

.fa {
  color: black;
}
</style>
