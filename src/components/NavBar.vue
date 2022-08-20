<template>
<nav class="navbar navbar-expand-lg navbar-light">
  <div class="container">
    <a class="navbar-brand" style="display: flex;" href="#"><img src="../../public/fav.png" style="width: 50px;"><h4 style="color: #00A2ED; font-weight: bold; margin-top: 8px;">Software</h4><h4 style="color: #04229B; font-weight: bold; margin-top: 8px;">Waffe</h4></a>
    <button class="navbar-toggler collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#navbarTogglerDemo02" aria-controls="navbarTogglerDemo02" aria-expanded="false" aria-label="Toggle navigation">
      <span  class="toggler-icon top-bar bbb2"></span>
      <span style="margin-left: 5px;" class="toggler-icon bbb middle-bar"></span>
      <span  class="toggler-icon bottom-bar bbb2"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarTogglerDemo02">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="#">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Link</a>
        </li>
        <li class="nav-item">
          <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a>
        </li>
      </ul>
      <form class="d-flex">
        <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
        <button class="btn btn-outline-success" type="submit">Search</button>
      </form>
    </div>
  </div>
</nav>
</template>

<script>
export default {
    name: 'NavBar'
}
</script>
<style scoped>

.navbar-toggler {
    border: 0 !important;
}

.navbar-toggler:focus,
.navbar-toggler:active,
.navbar-toggler-icon:focus {
    outline: none !important;
    box-shadow: none !important;
    border: 0 !important;
}

/* Lines of the Toggler */
.toggler-icon{
    width: 30px;
    height: 3px;
    background-color: #e74c3c;
    display: block;
    transition: all 0.2s;
}

/* Adds Space between the lines */
.middle-bar{
    margin: 5px auto;
}

/* State when navbar is opened (START) */
.navbar-toggler .top-bar {
    transform: rotate(45deg);
    transform-origin: 10% 10%;
}

.navbar-toggler .middle-bar {
    opacity: 0;
    filter: alpha(opacity=0);
}

.navbar-toggler .bottom-bar {
    transform: rotate(-45deg);
    transform-origin: 10% 90%;
}
/* State when navbar is opened (END) */

/* State when navbar is collapsed (START) */
.navbar-toggler.collapsed .top-bar {
    transform: rotate(0);
}

.navbar-toggler.collapsed .middle-bar {
    opacity: 1;
    filter: alpha(opacity=100);
}

.navbar-toggler.collapsed .bottom-bar {
    transform: rotate(0);
}
/* State when navbar is collapsed (END) */

/* Color of Toggler when collapsed */
.bbb{
    background-color: #04229B;
}
.bbb2{
    background-color: #00A2ED;
}
</style>

