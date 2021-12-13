<template>
  <footer>
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

        <!--FOOTER LINKS-->
        <div class="footer_links row">

            <!--ADDRESS-->
            <div class="col-6">
                <h3>Address</h3>
                <ul>
                    <li> 382 NE 191st ST # 87394 MIAMI, Fl 33179-3899</li>
                    <li>+1(305)547-9909(9am-5pm EST,Monday-Friday)</li>
                    <li>support@maxcoach-com</li> 
                </ul>
                <!--SOCIAL-->
                    <ul class="d-flex social">
                        <li><a href=""><i class="fab fa-facebook-square"></i></a></li>
                        <li><a href=""><i class="fab fa-twitter-square"></i></a></li>
                        <li><a href=""><i class="fab fa-instagram"></i></a></li>
                        <li><a href=""><i class="fab fa-linkedin"></i></a></li>
                    </ul>
            </div>

            <div class="col-3">
                <h3>Explore</h3>
                <ul>
                    <li v-for="(link,index) in exploreLinks" :key="`link${index}`" >
                    <a href="">
                    {{link}}
                    </a>
                    </li>
                </ul>
            </div>

            <div class="col-3">
                <h3>Information</h3>
                <ul>
                    <li v-for="(link,index) in informationLinks" :key="`link${index}`" >
                    <a href="">
                    {{link}}
                    </a>
                    </li>
                </ul>

            </div>
        </div>

      </div>
  </footer>
</template>

<script>
export default {
name:'Footer',
//LINKS ARRAY FROM APP
props:{
exploreLinks:Array,
informationLinks:Array,
}
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

/*FOOTER BUTTON*/
.footer_links{
li{
    color:$tertiary-color;
}
ul{
    padding-left:0;
    list-style-type: none;
    a{
        color:$tertiary-color;
        text-decoration: none;
        &:hover {
            color:$violet-color;
            }
    }
}
.social a{
    padding-right:20px;
    i{
        font-size:25px;
    }
}
    
}

</style>