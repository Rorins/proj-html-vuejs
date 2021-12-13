<template>
  <section>
 
      <div class="container">
      
      <!--TITLES-->
      <div class="text-center titles">
      <h2>STIMULATED TO LEARN?</h2>
      <h1>Featured Online Courses</h1>
      </div>

      <!--COURSES-->
      <div class="row courses">
          <div class="col-6 border_color d-flex">
              <div class="thumbnail bg_1">
              </div>
              <div>
              <p>$40.<span>00</span></p>
              <h5>Learning to Write as a Professional Author</h5>
              <span><i class="far fa-file-alt"></i>20 Lessons</span>
              <span><i class="far fa-user"></i>50 Students</span>
              </div>
          </div>

          <div class="col-6 border_color d-flex">
              <div class="thumbnail bg_2">
              </div>
              <div>
              <p>Free</p>
              <h5>Customer-centric Info-Tech Strategies</h5>
              <span><i class="far fa-file-alt"></i>24 Lessons</span>
              <span><i class="far fa-user"></i>769 Students</span>
              </div>
          </div>

          <div class="col-6 border_color d-flex">
              <div class="thumbnail bg_3">
              </div>
              <div>
              <p>$19.<span>00</span></p>
              <h5>Open Programming Courses for everyone:Python </h5>
              <span><i class="far fa-file-alt"></i>17 Lessons</span>
              <span><i class="far fa-user"></i>62 Students</span>
              </div>
          </div>
          
          <div class="col-6 border_color d-flex">
              <div class="thumbnail bg_4">
              </div>
              <div>
              <p>$26.<span>00</span></p>
              <h5>Academic Listening and Note-taking</h5>
              <span><i class="far fa-file-alt"></i>14 Lessons</span>
              <span><i class="far fa-user"></i>67 Students</span>
              </div>
          </div>
          <div class="col-6 border_color d-flex">
              <div class="thumbnail bg_5">
              </div>
              <div>
              <p>$39.<span>00</span></p>
              <h5>Master JQuery in a Short Period of Time</h5>
              <span><i class="far fa-file-alt"></i>6 Lessons</span>
              <span><i class="far fa-user"></i>51 Students</span>
              </div>
          </div>
          <div class="col-6 border_color d-flex">
              <div class="thumbnail bg_6">
              </div>
              <div>
              <p>$59.<span>00</span></p>
              <h5>Introduction to Javascript for Beginners</h5>
              <span><i class="far fa-file-alt"></i>14 Lessons</span>
              <span><i class="far fa-user"></i>76 Students</span>
              </div>
          </div>
      </div>
      <div class="d-flex justify-content-center">
      <button class="button">View all courses<i class="fas fa-arrow-right"></i></button>
      </div>
      </div>

      </section>
</template>

<script>
export default {
name:'SectionOne'
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';

section{
    background-color:#f5f7fa;
    .titles, & div:nth-last-child(1){
        padding:60px 0;
    }
        h1{
            color:$violet-color;
        }
        h2{
            color:$tertiary-color;
            font-size:20px;
        }
        /*COURSES*/
        .courses div{
        padding: 40px 25px;
        p{
            color:$secondary-color;
            font-weight:bolder;
            font-size:25px;
            span{
                font-size:20px;
                color:$secondary-color;
            }
        }
        .thumbnail{
            width:200px;
            height: 200px;
            border-radius:50%;
            background-position: center;
            background-size:300px;
        }
        /*BACKGROUNDS*/
        .bg_1{
            background-image: url(../assets/course-02-480x298.jpg);
        }
        .bg_2{
            background-image: url(../assets/stock-full-hd-03-480x298.jpg);
        }
        .bg_3{
            background-image: url(../assets/stock-full-hd-04-480x298.jpg);
        }
        .bg_4{
            background-image: url(../assets/stock-full-hd-06-480x298.jpg);
        }
        .bg_5{
            background-image: url(../assets/course-featured-image-01-480x298.jpg);
        }
        .bg_6{
            background-image: url(../assets/stock-full-hd-05-480x298.jpg);
        }
        h5{
            color:$violet-color;
        }
        span{
            color:$tertiary-color;
            margin-right:10px;
            i{
                padding-right:5px;
            }
            
        }
        }
        
    /*BUTTON*/
    & div:nth-last-child(1) button{
        .fa-arrow-right{
            padding-left:5px;
        }
    }
};
    
    
    
</style>