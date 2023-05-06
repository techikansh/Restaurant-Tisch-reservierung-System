<script setup></script>
<template>
  <nav class="navbar sticky-top navbar-expand-md navbar-light">
    <div class="container">
      <a class="navbar-brand me-5" href="#"
        ><img alt="Vue logo" class="logo" src="../assets/oliveWood3.png"/>
      </a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>





      <div class="collapse navbar-collapse ms-5" id="navbarSupportedContent">

        <ul class="navbar-nav me-auto my-2 my-lg-0" style="background-color: ; text-align: center">
          <li class="nav-item me-4">
            <router-link class="nav-link-home" id="links" :to="{ name: 'home' }">Home</router-link>
          </li>
          <li class="nav-item me-4">
            <router-link class="nav-link-uns" id="links" :to="{ name: 'ueber-uns' }"
              >About Us</router-link
            >
          </li>

          <li class="nav-item me-4">
            <router-link class="nav-link-contact" id="links" :to="{ name: 'kontakt' }">Contact</router-link>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>


<style scoped>
#links {
  color: #ffffff;
  font-size: 20;
  font-weight: 800;
}
#links:hover {
  color: #F8B333;
}

header{
  position : relative;
  overflow: hidden;
}

header .logo {
  position: absolute;
  top:10%;
  left: 3%;
  width: 300px;
  height : 300px;
  object-fit: cover;
  transform: translate(-10%, -30%);
}






header li .nav-link-home{
  color: #F8B333;
  font-size : 25px;
  font-family: 'BoucherieCursive', bold, cursive;
  position: absolute;
  top: 140%;
  right: 10%;
  /* transform: translate(50%, 195%); */
  /* float : right; */
}

header li .nav-link-uns{
  color: #F8B333;
  position: absolute;
  top: 140%;
  right: 14%;
  font-family: 'BoucherieCursive', bold, cursive;
  font-size : 25px;
  /* transform: translate(40%, 195%); */
  /* float : right; */
}

header li .nav-link-contact{
  color: #F8B333;
  position: absolute;
  top: 140%;
  right: 20%;
  font-family: 'BoucherieCursive', bold, cursive;
  font-size : 25px;
  /* transform: translate(30%, 195%); */
  /* float : right; */
}

</style>
