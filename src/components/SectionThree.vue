<template>
<section>
<div class="container">

<div class="row">
  <!--FIRST COLUMN-->
    <div class="col-8">
      <!--DECORATION AND IMAGES-->
      <img src="../assets/maxcoach-shape-05.png" alt="">
      <img src="../assets/maxcoach-shape-07.png" alt="">
      <img src="../assets/home-2-popup-video-poster.jpg" alt="">
      <img class="youtube_btn" src="../assets/icon-youtube-play.png" alt="">
    </div>

  <!--SECOND COLUMN-->
    <div class="info col-4 d-flex flex-column justify-content-center">
       <i class="far fa-circle"></i>
        <h3>GET STARTED <span>EFFORTLESSLY</span></h3>
        <h1>Enjoy our <span>Companionship</span></h1>
        <p>Sneek peek into what has in store for you on our online teaching and mentoring portal.Seek for some hidden hints of early-bird rewards as well.</p>
        <p><a href="">Download free guidebook<i class="fas fa-arrow-right"></i></a></p>
    </div>
</div>

</div>
</section>
</template>

<script>
export default {
name:'SectionThree'
}
</script>


<style scoped lang="scss">
@import '@/styles/variables';


/*FIRST-COLUMN*/
.row div:first-child{
  padding:100px 70px;
  position:relative;
  img{
      width: 100%;
  }
  .youtube_btn{
    width:120px;
    position:absolute;
    top:50%;
    left:50%;
    &:hover {
    cursor: pointer;
    width:130px;
  }
  }
  
/*DECORATION*/
  img:nth-child(1){
    width:180px;
    position:absolute;
    top:150px;
    left:0;
    z-index:-1;
  }
  img:nth-child(2){
    width:160px;
    position:absolute;
    bottom:0;
    right:0;
    z-index:-1;
  }
}



/*SECOND-COLUMN*/
.info {
  position:relative;
.fa-circle{
        position:absolute;
        left:0;
        top:80px;
        color:#efcfba;
        font-size:60px;
    }
h3 {
  font-size:20px;
  color:$tertiary-color;
  span {
    color:$violet-color;
  }
}
h1{
  color:$violet-color;
  span {
    color:$primary-color;
    font-weight:300;
    }
}
p a{
  text-decoration: none;
  color:$primary-color;
  border-bottom:1px solid gray;
  &:hover {
    cursor: pointer;
    color:$violet-color;
  }
}
}
</style>