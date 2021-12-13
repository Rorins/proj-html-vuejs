<template>
  <section>
      <div class="container">
          
          <div class="row">

              <div class="titles col-4">
                  <h3>ENJOYABLE INSIGHTS</h3>
                  <h2>Most Viewed <span>Best Blogs</span></h2>
                  
                  <!--CARD WITH LIST-->
                  <ul>
                      <li v-for="(element,index) in list " :key="`element${index}`">
                        <i :class="element.icon"></i>
                        <span>{{element.listItem}}</span>
                      </li>
                  </ul>
              </div>
              
              <!--CARDS-->
              <div class="col-4 card_container">
                  <div class="card">
                      <div><img src="../assets/artist-blog-03-480x352.jpeg" alt=""></div>
                      <div class="description">
                      <h3>ARTIST</h3>
                      <h2>Brush Strokes Energize Trees in Paintings</h2>
                      <span><i class="far fa-calendar"></i>May 15,2020</span>
                      <span><i class="far fa-eye"></i>688 views</span>
                      </div>
                    </div>
              </div>

              <div class="col-4 card_container">
                      <div class="card">
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
      </div>
  </section>
</template>

<script>
export default {
name:'SectionSix',
data(){
    return{
        list:[
            {
                icon:"fas fa-arrow-right",
                listItem:"Become a better Blogger:Content Planning",
            },
            {
                icon:"fas fa-arrow-right",
                listItem:"Promoting your Online Business on Pinterest",
            },
             {
                icon:"fas fa-arrow-right",
                listItem:"Gamification and Game-Based Learing",
            },
             {
                icon:"fas fa-arrow-right",
                listItem:"Designing an Online Course from Expert's Perspective",
            },
             {
                icon:"fas fa-arrow-right",
                listItem:"Why Online Courses are the Future of Education",
            }
        ]
    }
}
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
.card_container{
    padding:0;
    .card{
        background-color:white;
        border:30px solid #f4f0ec;
        img{
    width: 100%;
    object-fit:cover,
    }
    .description{
    padding:30px;
    h2{
        color:$violet-color;;
    }
    h2,h3{
        font-size:20px;
    }
    h3,span{
        font-weight:300;
        color:$tertiary-color;
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
}


</style>