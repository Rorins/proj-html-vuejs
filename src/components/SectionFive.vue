<template>
  <section>
      <div class="container">
          <div class="row text-center">
            
            <!--TITLES-->
              <div class="titles">
                <h3>Start today for getting <span>Online Certification</span></h3>
                <h1>You can be your own guiding star with our help!</h1>
                <button class="button">Get started now</button>
              </div>
            
            <!--NUMBERS-->
            <div class="col-3">
                <h3>Successfully trained</h3>
                <h2>1790</h2>
                <p>Enrolled Learners</p>
            </div>

            <div class="col-3">
                <h3>Proudly Received</h3>
                <h2>1790</h2>
                <p>Enrolled Learners</p>
            </div>

            <div class="col-3">
                <h3>Firmly Established</h3>
                <h2>1790</h2>
                <p>Enrolled Learners</p>
            </div>

            <div class="col-3">
                <h3>Getting Featured on</h3>
                <h2>1790</h2>
                <p>Enrolled Learners</p>
            </div>
            
          </div>
      </div>
  </section>
</template>

<script>
export default {
name:'SectionFive'
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';

.titles{
h3{
    font-size:20px;
    span{
        color:$primary-color;
        font-weight:300;
    }
}
h1, h3{
    color:$violet-color;   
    }
}


</style>