<template>
  <section>
      <div class="container">
          
          <div class="row">

              <div class="col-4">
                  <h3>ENJOYABLE INSIGHTS</h3>
                  <h2>Most Viewed <span>Best Blogs</span></h2>

                  <ul>
                      <li>Become a better Blogger:Content Planning</li>
                      <li>Promoting your Online Business on Pinterest</li>
                      <li>Gamification and Game-Based Learing</li>
                      <li>Designing an Online Course from Expert's Perspective</li>
                      <li>Why Online Courses are the Future of Education</li>
                  </ul>
              </div>
              
              <!--CARDS-->
              <div class="col-4">
                      <div><img src="../assets/artist-blog-03-480x352.jpeg" alt=""></div>
                      <h3>ARTIST</h3>
                      <h2>Brush Strokes Energize Trees in Paintings</h2>
                      <span>May 15,2020</span>
                      <span>688 views</span>
              </div>

              <div class="col-4">
                      <div><img src="../assets/artist-blog-01-480x352.jpg" alt=""></div>
                      <h3>ARTIST</h3>
                      <h2>Brush Strokes Energize Trees in Paintings</h2>
                      <span>May 15,2020</span>
                      <span>688 views</span>
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

img{
    width: 100%;
    object-fit:cover,
}

</style>