<template>
  <header>

<!--NAVBAR-->
<nav class="navbar navbar-expand-lg navbar-light bg-light">
<div class="container">

<!--lOGO-->
<div>
  <a class="navbar-brand" href="#"><img src="../assets/dark-logo.png" alt="MaxCoach"></a>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>
</div>

<!--LINKS-->
<div>
  <div class="collapse navbar-collapse" id="navbarSupportedContent">
    <ul class="navbar-nav mr-auto">
      <li class="nav-item dropdown">
        <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
          Home
        </a>
        <!-- <div class="dropdown-menu" aria-labelledby="navbarDropdown">
          <a class="dropdown-item" href="#">Action</a>
          <a class="dropdown-item" href="#">Another action</a>
          <div class="dropdown-divider"></div>
          <a class="dropdown-item" href="#">Something else here</a>
        </div> -->
      </li>
      <li class="nav-item dropdown">
        <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
          Pages
        </a>
      </li>
       <li class="nav-item dropdown">
        <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
          Courses
        </a>
      </li>
       <li class="nav-item dropdown">
        <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
          Features
        </a>
      </li>
       <li class="nav-item dropdown">
        <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
          Blog
        </a>
      </li>
       <li class="nav-item dropdown">
        <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
          Shop
        </a>
      </li>

   <!--SEARCH-BAR-->   
    </ul>
    <div class="search">
              <div class="input-group mb-3">
                <input
                  type="text"
                  class="form-control border-0"
                  placeholder="Search.."
                  aria-label=""
                  aria-describedby="basic-addon1"
                />
                <div class="input-group-prepend">
                  <button class="btn" type="button">
                    <i class="fas fa-search"></i>
                  </button>
                </div>
              </div>
    </div>
    </div>

  </div>
</div>
</nav>
</header>
</template>

<script>
export default {
name:'Header'
}
</script>

<style scoped lang="scss">
li{
    padding-right:20px;
}

</style>