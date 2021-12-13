<template>
  <section>
      <div class="container">

        <!--TITLES-->
      <div class="titles text-center">
      <h3>MAXCOACH AVAILABLE COURSES</h3>
      <h2>Access <span>Smart Tutoring</span> Program For Benefits.</h2>
      </div>

      <div class="row">

          <!--CARDS-->
          <div v-for="(card,index) in cards" :key="`card${index}`" class="col-4">
          <img :src="require(`../assets/${card.image}`)" :alt="card.title">
          <h3>{{card.title}}</h3>
          <p>{{card.details}}</p>
          <p><a href="">{{card.button}}<i class="fas fa-arrow-right"></i></a></p>
          </div>

      </div>
      </div>
  </section>
</template>

<script>
export default {
name:'SectionTwo',
data(){
  return{
    cards:[
      {
        image:"home-2-image-box-01.png",
        title:"Customize Preferences",
        details:"Learners are given the right to arrange and customize their study schedule and timetable based on preferences.",
        button:"Start here",
      },
      {
        image:"about-us-02-image-box-02.png",
        title:"Cloud Storage",
        details:"You can store online lessons via online cloud or download to your device and revise lessons on the way.",
        button:"Get Free Quote",
      },
      {
        image:"home-2-image-box-03.png",
        title:"Multimedia Channels",
        details:"We provide study materials with various formats: video,audio,slids,doc,prints,books and applications.",
        button:"Start now",
      },
    ]
  }
}
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';

/*TITLES*/
.titles{
  padding:60px 0;
  h3{
    font-size:20px;
    color:$tertiary-color;
  }
  span{
    color:$primary-color;
    font-weight:300;
  }
}

/*CARDS*/
img{
  padding-bottom:30px;
}
p,a{
    color:$tertiary-color;
    a{
      text-decoration: none;
      color:$darkGray-color;
      &:hover{
        color:$violet-color;
        }
    }
  }
</style>