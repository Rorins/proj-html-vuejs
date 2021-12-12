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
                <p>ENROLLED LEARNERS</p>
            </div>

            <div class="col-3">
                <h3>Proudly Received</h3>
                <h2>19</h2>
                <p>COUNTRYWIDE AWARDS</p>
            </div>

            <div class="col-3">
                <h3>Firmly Established</h3>
                <h2>24</h2>
                <p>LOCAL BRANCHES</p>
            </div>

            <div class="col-3">
                <h3>Getting Featured on</h3>
                <h2>1090</h2>
                <p>BLOG POSTS</p>
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

/*TITLES*/
.titles{
padding:50px 0;
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

/*NUMBERS*/
.col-3{
    border: 1px solid $tertiary-color;
    padding:90px 50px;
    h3{
        color:$violet-color;
    }
    h2{
        color:$primary-color;
        font-weight:bolder;
    }
    p{
        color:$tertiary-color;
    }
}


</style>