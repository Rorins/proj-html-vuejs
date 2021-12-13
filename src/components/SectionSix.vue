<template>
  <section>
      <div class="container">
          
          <div class="row">

              <div class="titles col-4">
                  <h3>ENJOYABLE INSIGHTS</h3>
                  <h2>Most Viewed <span>Best Blogs</span></h2>
                  
                  <!--CARD WITH LIST-->
                  <ul>
                      <li><i class="fas fa-arrow-right"></i>Become a better Blogger:Content Planning</li>
                      <li><i class="fas fa-arrow-right"></i>Promoting your Online Business on Pinterest</li>
                      <li><i class="fas fa-arrow-right"></i>Gamification and Game-Based Learing</li>
                      <li><i class="fas fa-arrow-right"></i>Designing an Online Course from Expert's Perspective</li>
                      <li><i class="fas fa-arrow-right"></i>Why Online Courses are the Future of Education</li>
                  </ul>
              </div>
              
              <!--CARDS-->
              <div class="col-4 card">
                      <div><img src="../assets/artist-blog-03-480x352.jpeg" alt=""></div>
                      <div class="description">
                      <h3>ARTIST</h3>
                      <h2>Brush Strokes Energize Trees in Paintings</h2>
                      <span><i class="far fa-calendar"></i>May 15,2020</span>
                      <span><i class="far fa-eye"></i>688 views</span>
                      </div>
              </div>

              <div class="col-4 card">
                      <div><img src="../assets/artist-blog-01-480x352.jpg" alt=""></div>
                      <div class="description">
                      <h3>ARTIST</h3>
                      <h2>Brush Strokes Energize Trees in Paintings</h2>
                      <span><i class="far fa-calendar"></i>May 15,2020</span>
                      <span><i class="far fa-eye"></i>688 views</span>
                      </div>
              </div>
          </div>
      </div>
  </section>
</template>

<script>
export default {
name:'SectionSix'
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';
section{
    padding:100px 0;
    background-color: #f5f1ed;
}

/*TITLES*/
.titles{
h3{
    color:$tertiary-color;
    font-size:20px;
}
h2{
    color:$violet-color;
    padding-bottom:20px;
    span{
        color:$primary-color;
        font-weight:300;
    }
    }
}

/*LIST*/
ul{
    list-style-type: none;
    padding-left:0;
    li{
        color:$violet-color;
        padding-bottom:20px;
        i{
            padding-right:15px;
        }
    }
}

/*CARDS*/
.card{
    background-color:white;
    .description{
    padding:30px;
    h2,h3{
        color:$violet-color;
        font-size:20px;
    }
    h3,span{
        font-weight:300;
    }
    span{
        color:$tertiary-color;
        font-size:20px;
        padding:10px;
        i{
            padding-right:10px;
        }
    }
    } 
}
img{
    width: 100%;
    object-fit:cover,
    }

</style>