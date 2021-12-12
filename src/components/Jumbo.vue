<template>
  <section>
<div class="container">
    <div class="row">
        <!--FIRST COLUMN-->
        <div class="col-6 first_column d-flex flex-column justify-content-center">
            <h1>Distant learning for further expansion</h1>
            <p>Leaning is a life-long journey that in fact we never find the terminate stop.Stop searching,enjoy the process.</p>
            <button class="button">
            <i class="fas fa-download"></i>
            <span>Download free guide</span>
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
             <img class="about_me" src="../assets/about-me-profile-ohm4dxoearqbxny7q3bq1pzbdgofdx0tobbeqcvzd0.jpg" alt="girl">
             <img src="../assets/maxcoach-shape-02.png" alt="circle">
             <img src="../assets/maxcoach-shape-08.png" alt="square">
             <img src="../assets/maxcoach-shape-08.png" alt="square">
             <img src="../assets/maxcoach-shape-07-150x150.png" alt="square">
             <i class="far fa-circle"></i>
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
.container .first_column{
    padding-right:140px;
    h1{
        color:$violet-color;
    }
    p{
        color:$tertiary-color;
    }
        a{
            text-decoration: none;
            color:$secondary-color;
            font-weight: bold;   
            border-bottom:1px solid  #919191;
        &:hover{
        color:$violet-color;
        }
        }
    .fa-download{
        padding-right:10px;
    }
    .button{
        width:300px;
        margin:20px 0;
        span{
            color:white;
            font-weight: bold;
            font-size:15px;
        }
    }
}
    
    

/*SECOND COLUMN*/
.second_column{
    .about_me{
        width:570px;
        border-radius:50%;
    }
    position:relative;
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
    .fa-circle{
        position:absolute;
        left:0;
        bottom:90px;
        color:#efcfba;
        font-size:60px;
    }
}
    


/*LOGOS*/
.logos{
    margin: 50px 0;
    img{
        filter:brightness(1.4) grayscale(1.2)
    }
}
    
   
    
</style>