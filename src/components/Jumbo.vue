<template>
  <section>
<div class="container">
    <div class="row">
        <!--FIRST COLUMN-->
        <div class="col-6 d-flex flex-column justify-content-center">
            <h1>Distant learning for further expansion</h1>
            <p>Leaning is a life-long journey that in fact we never find the terminate stop.Stop searching,enjoy the process.</p>
            <button class="button">
            <i class="fas fa-download"></i>
            Download free guide
            </button>
            <p>Have questions?
                <a href="">
                <span>Get free sample 
                    <i class="fas fa-arrow-right"></i>
                </span> 
                </a>
            </p>
        </div>
       
       <!--SECOND COLUMN-->
        <div class="col-6 second_column">
             <img class="about_me" src="../assets/about-me-profile-ohm4dxoearqbxny7q3bq1pzbdgofdx0tobbeqcvzd0.jpg" alt="">
             <img src="../assets/maxcoach-shape-02.png" alt="">
             <img src="../assets/maxcoach-shape-08.png" alt="">
             <img src="../assets/maxcoach-shape-08.png" alt="">
             <img src="../assets/maxcoach-shape-07-150x150.png" alt="">
        </div>
    </div>
 
    <!--LOGOS-->
    <div class="row logos">
        <div class="col-2"><img src="../assets/client-logo-01.png" alt=""></div>
        <div class="col-2"><img src="../assets/client-logo-02.png" alt=""></div>
        <div class="col-2"><img src="../assets/client-logo-03.png" alt=""></div>
        <div class="col-2"><img src="../assets/client-logo-04.png" alt=""></div>
        <div class="col-2"><img src="../assets/client-logo-05.png" alt=""></div>
        <div class="col-2"><img src="../assets/client-logo-06.png" alt=""></div>
    </div>

</div>
  </section>
</template>

<script>
export default {
name:'Jumbo'
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';

/*FIRST COLUMN*/
.container div:first-child{
    padding-right:140px;
}
    h1{
        color:$violet-color;
    }
    p{
        color:$terziary-color;
    }
        a{
            text-decoration: none;
            color:$secondary-color;
            font-weight: bold;   
            border-bottom:1px solid  #919191;
        &:hover{
        color:rgb(58, 56, 56);
        }
        }
    .fa-download{
        padding-right:10px;
    }
    .button{
        width:300px;
        margin:20px 0;
    }
    

/*SECOND COLUMN*/
.second_column{
    position:relative;
}
    img:nth-child(2){
        position:absolute;
        top:100px;
    }
    img:nth-child(3){
        position:absolute;
        top:100px;
        left:0;
        z-index:-1;
    }
    img:nth-child(4){
        position:absolute;
        top:250px;
        left:0;
        z-index:-1;
    }
    img:nth-child(5){
        position:absolute;
        bottom:30px;
        right:10px;
        z-index:-1;
    }
.about_me{
        width:570px;
        border-radius:50%;
    }

/*LOGOS*/
.logos{
    margin: 50px 0;
}
</style>