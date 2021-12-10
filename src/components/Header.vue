<template>
  <header>

<!--NAVBAR-->
<nav class="navbar navbar-expand-lg navbar-light">
<div class="container">

<!--lOGO-->
<div>
  <a class="navbar-brand" href="#"><img class=logo src="../assets/dark-logo.png" alt="MaxCoach"></a>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>
</div>

<!--LINKS-->
<div>
  <div class="collapse navbar-collapse" id="navbarSupportedContent">
    <ul class="navbar-nav mr-auto">
      <li class="nav-item dropdown">
        <a class="nav-link dropdown-arrow" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
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
        <a class="nav-link dropdown-arrow" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
          Pages
        </a>
      </li>
       <li class="nav-item dropdown">
        <a class="nav-link dropdown-arrow" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
          Courses
        </a>
      </li>
       <li class="nav-item dropdown">
        <a class="nav-link dropdown-arrow" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
          Features
        </a>
      </li>
       <li class="nav-item dropdown">
        <a class="nav-link dropdown-arrow" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
          Blog
        </a>
      </li>
       <li class="nav-item dropdown">
        <a class="nav-link dropdown-arrow" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
          Shop
        </a>
      </li>
      <li>
        <a class="user_icon" href="">
          <i class="far fa-user-circle"></i>
          </a>
      </li>
      </ul>

    <!--SEARCH-BAR--> 
    <div class="search">
              <div class="input-group">
                <input
                  type="text"
                  class="form-control border-0"
                  placeholder="Search..."
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
@import '@/styles/variables';
.logo{
width:180px;
}
 
 /*NAVBAR*/

.navbar-light{
background-color: #fff;
/*LIST ITEMS*/
  li{
    padding-right:20px;
 }
 .nav-link, a{
   color:$darkGray-color;
 }
 .dropdown-arrow::after{
  font-family: FontAwesome;
  font-weight: 600;
  content: '\f078';
 }
.user_icon i{
  font-size: 20px;
  padding-top:10px;
  &:hover{
  color:rgba(0, 0, 0, 0.7);
}
}
}

/*SEARCH*/
.search{
  width: 250px;
  .form-control, .btn{
    background-color: #f5f5f5;
    padding:10px 20px;
  }
    .fa-search{
      color:$secondary-color;
    }
}
  

</style>