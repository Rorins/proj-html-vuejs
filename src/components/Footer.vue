<template>
  <footer>
      <div class="container">

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
                        <li v-for="(link,index) in social" :key="`link${index}`">
                            <a href=""><i :class="link"></i></a>
                            </li>
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

            <!--COPYRIGHT-->
            <div class="copyright text-center">
            <span>
                <i class="far fa-copyright"></i>
                Maxcoach,All Rights Reserved
            </span>
            <!--ARROW BUTTON-->
            <a href="">
                <div class="arrow_button d-flex align-items-center justify-content-center">
                <i class="fas fa-arrow-up"></i>
                </div>
            </a>
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
},
data(){
    return{
        social:[
            "fab fa-facebook-square",
            "fab fa-twitter-square",
            "fab fa-instagram",
            "fab fa-linkedin",
        ]
    }
}
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';

/*FOOTER*/
footer{
    background-color:#f8f8f8;
    position:relative;
    div{
        padding:30px 0;
    }
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
/*SOCIAL*/
.social a{
    padding-right:20px;
    i{
        font-size:25px;
    }
}
}
.copyright span{
    color:$tertiary-color;
}
}
.arrow_button{
    width: 60px;
    height:60px;
    border-radius: 50%;
    background-color:$primary-color;
    position:absolute;
    right:10px;
    color:white;
}

</style>