<template>
  <footer>
      <div class="container">

        <!--FOOTER LINKS-->
        <div class="footer row">

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

footer{
    background-color:#f8f8f8;
    div{
        padding:20px 0;
    }
}

/*FOOTER*/
.footer{
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