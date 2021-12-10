<template>
  <section>
      <!--COURSES-->
      <div class="container">
      
      <div class="text-center titles">
      <h2>STIMULATED TO LEARN?</h2>
      <h1>Featured Online Courses</h1>
      </div>

      <div class="row courses">
          <div class="col-6 d-flex">
              <div class="thumbnail">
              </div>
              <div>
              <p>$40.<span>00</span></p>
              <h5>Learning to Write as a Professional Author</h5>
              <span>20 Lessons</span>
              <span>50 Students</span>
              </div>
          </div>
          <div class="col-6 d-flex">
              <div class="thumbnail">
              </div>
              <div>
              <p>Free</p>
              <h5>Learning to Write as a Professional Author</h5>
              <span>24 Lessons</span>
              <span>769 Students</span>
              </div>
          </div>
          <div class="col-6 d-flex">
              <div class="thumbnail">
              </div>
              <div>
              <p>$19.<span>00</span></p>
              <h5>Learning to Write as a Professional Author</h5>
              <span>17 Lessons</span>
              <span>62 Students</span>
              </div>
          </div>
          <div class="col-6 d-flex">
              <div class="thumbnail">
              </div>
              <div>
              <p>$26.<span>00</span></p>
              <h5>Learning to Write as a Professional Author</h5>
              <span>14 Lessons</span>
              <span>67 Students</span>
              </div>
          </div>
          <div class="col-6 d-flex">
              <div class="thumbnail">
              </div>
              <div>
              <p>$39.<span>00</span></p>
              <h5>Learning to Write as a Professional Author</h5>
              <span>6 Lessons</span>
              <span>51 Students</span>
              </div>
          </div>
          <div class="col-6 d-flex">
              <div class="thumbnail">
              </div>
              <div>
              <p>$59.<span>00</span></p>
              <h5>Learning to Write as a Professional Author</h5>
              <span>14 Lessons</span>
              <span>76 Students</span>
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
            background-image: url(../assets/course-02-480x298.jpg);
            border-radius:50%;
            background-position: center;
        }
        h5{
            color:$violet-color;
        }
        span{
            color:$tertiary-color;
            margin-right:10px;
            
        }
        }
        
    /*BUTTON*/
    & div:nth-last-child(1) button{
        width:260px;
        .fa-arrow-right{
            padding-left:5px;
        }
    }
};
    
    
    
</style>