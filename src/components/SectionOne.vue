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
              <p>$40.00</p>
              <h5>Learning to Write as a Professional Author</h5>
              <span>20 Lessons</span>
              <span>50 Students</span>
              </div>
          </div>
          <div class="col-6 d-flex">
              <div class="thumbnail">
              </div>
              <div>
              <p>$40.00</p>
              <h5>Learning to Write as a Professional Author</h5>
              <span>20 Lessons</span>
              <span>50 Students</span>
              </div>
          </div>
          <div class="col-6 d-flex">
              <div class="thumbnail">
              </div>
              <div>
              <p>$40.00</p>
              <h5>Learning to Write as a Professional Author</h5>
              <span>20 Lessons</span>
              <span>50 Students</span>
              </div>
          </div>
          <div class="col-6 d-flex">
              <div class="thumbnail">
              </div>
              <div>
              <p>$40.00</p>
              <h5>Learning to Write as a Professional Author</h5>
              <span>20 Lessons</span>
              <span>50 Students</span>
              </div>
          </div>
          <div class="col-6 d-flex">
              <div class="thumbnail">
              </div>
              <div>
              <p>$40.00</p>
              <h5>Learning to Write as a Professional Author</h5>
              <span>20 Lessons</span>
              <span>50 Students</span>
              </div>
          </div>
          <div class="col-6 d-flex">
              <div class="thumbnail">
              </div>
              <div>
              <p>$40.00</p>
              <h5>Learning to Write as a Professional Author</h5>
              <span>20 Lessons</span>
              <span>50 Students</span>
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
            color:$terziary-color;
            font-size:20px;
        }
        /*COURSES*/
        .courses div{
        padding: 40px 25px;
        p{
            color:$secondary-color;
            font-weight:bold;
            font-size:25px;
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
            color:$terziary-color;
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