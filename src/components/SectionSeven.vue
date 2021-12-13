<template>
<section>

    <div class="container">
        <!--SUBSCRIBE-->
          <div class="subscribe row d-flex justify-content-center text-center">

              <h2>Subscribe <span>Newsletters</span></h2>
              <h3>Enter your email address to register to our newsletter subscription delivered on a regular basis!</h3>
              <!--DETAILS-->
              <img class="circle" src="../assets/maxcoach-shape-02.png" alt="circle">
              
              <!--SUBSCRIBE BUTTON-->
              <div class="input-group mb-3">
                <input type="text" class="form-control" placeholder="Enter your email" aria-label="email" aria-describedby="button-addon2">
                <div class="input-group-append">
                <button class="btn btn-outline-secondary" type="button" id="button-addon2">Subscribe</button>
                </div>
            </div>

          </div>
    </div>

</section>
</template>

<script>
export default {
name:'SectionSeven'
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';

/*SUBSCRIBE*/
.subscribe{
position:relative;
padding:80px 350px;
h2{
    color:$violet-color;
    span{
        color:$primary-color;
    }
}
h3{
    color:$tertiary-color;
    font-size:20px;
    padding-bottom:40px;
}
.circle{
    position:absolute;
    right:20px;
    width:160px;
}


/*SUBSCRIBE BUTTON*/
.input-group{
    width: 600px;
    input{
        background-color:#f5f5f5;
        border:none;
        padding:10px;
    }
    button{
        background-color:$secondary-color;
        border:none;
        color:white;
        padding:10px;
    }
}
}

</style>