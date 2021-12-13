<template>
  <section>
      <div class="container">
          <div class="row text-center">
            
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


/*NUMBERS*/
.col-3{
    border: 1px solid #f5f1ed;
    padding:90px 50px;
    h3{
        color:$violet-color;
    }
    h2{
        color:$primary-color;
        font-weight:bolder;
        font-size:70px;
    }
    p{
        color:$tertiary-color;
        font-weight:bold;
    }
}


</style>