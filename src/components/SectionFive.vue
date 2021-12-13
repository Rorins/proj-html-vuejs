<template>
  <section>
      <div class="container">

          <!--NUMBERS-->
          <div class="row text-center">
            <div v-for="(data,index) in data " :key="`data${index}`" class="col-3">
                <h3>{{data.title}}</h3>
                <h2>{{data.number}}</h2>
                <p>{{data.subtitle}}</p>
            </div>

          </div>
      </div>
  </section>
</template>

<script>
export default {
name:'SectionFive',
data(){
    return{
        data:[
            {
                title:"Successfully trained",
                number:"1790",
                subtitle:"ENROLLED LEARNERS",
            },
            {
                title:"Proudly received",
                number:"19",
                subtitle:"COUNTRYWIDE AWARDS",
            },
            {
                title:"Firmly Established",
                number:"24",
                subtitle:"LOCAL BRANCHES",
            },
            {
                title:"Getting Featured on",
                number:"1090",
                subtitle:"BLOG POSTS",
            },

        ]
    }
}
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