<template>
  <section>
      <div class="container">

      <div class="titles text-center">
      <h3>MAXCOACH AVAILABLE COURSES</h3>
      <h2>Access <span>Smart Tutoring</span> Program For Benefits.</h2>
      </div>

      <div class="row">
          <div class="col-4"><img src="../assets/home-2-image-box-01.png" alt="">
          <h3>Customize Preferences</h3>
          <p>Learners are given the right to arrange and customize their study schedule and timetable based on preferences.</p>
          <p><a href="">Start here<i class="fas fa-arrow-right"></i></a></p>
          </div>

          <div class="col-4"><img src="../assets/about-us-02-image-box-02.png" alt="">
          <h3>Cloud Storage</h3>
          <p>You can store online lessons via online cloud or download to your device and revise lessons on the way.</p>
          <p><a href="">Get Free Quote<i class="fas fa-arrow-right"></i></a></p>
          </div>

          <div class="col-4"><img src="../assets/home-2-image-box-03.png" alt="">
          <h3>Multimedia Channels</h3>
          <p>We provide study materials with various formats: video,audio,slids,doc,prints,books and applications.</p>
          <p><a href="">Start now<i class="fas fa-arrow-right"></i></a></p>
          </div>

      </div>
      </div>
  </section>
</template>

<script>
export default {
name:'SectionTwo'
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';
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
img{
  padding-bottom:30px;
}
p,a{
    color:$tertiary-color;
    a{
      text-decoration: none;
      color:$darkGray-color;
    }
  }
</style>