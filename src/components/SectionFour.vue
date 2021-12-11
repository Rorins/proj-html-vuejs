<template>
  <section>
      <div class="container">
          <div class="row">
        
            <!--TITLES-->
            <div class="titles text-center">
                <h3>GREAT WORDS ABOUT MAXCOACH</h3>
                <h1>Our <span>top learners'</span> verbatism</h1>
            </div>
            
            <!--REVIEW CARDS-->
            <div class="col-4" v-for="(review,index) in reviews" :key="`review${index}`">
                <Card :title="review.title"
                 :text="review.text" 
                 :image="review.image"
                :subtext="review.author"
                 :subtextTwo="review.job"/>
            </div>
    
      </div>

<!--CIRCLE BAR-->
<div class="d-flex justify-content-center circle_bar">
<div></div>
<div></div>
<div></div>
<div></div>
</div>

    </div>
  </section>
</template>

<script>
import Card from '@/components/Card.vue'
export default {
name:'SectionFour',
components:{
    Card,
},
data(){
    return{
        //LIST OF REVIEW CARDS
        reviews:[
            {
                title: "It's a choice of quality for people with special needs",
                text: "I'm a very strict person so I require everything to be organized and neat.Then,I'll be able to make things right and shine.MaxCoach guys just got me.",
                image: "testimonial-avata-03",
                author:"FLORENCE THEMES",
                job:"/Multimedia Admin"
            },
            {
                title: "High level of efficiency and scientific teaching methods",
                text: "I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus.Great study portal for people like me.",
                image: "testimonial-avata-02",
                author:"MINA HOLLACE",
                job:"/Freelancer"
            },
            {
                title: "Professional team of specialists and passioante mentors at reach",
                text: "I need to get a certificate for English proficiency and MaxCoach is my best choice.Their tutors are smart and professional when dealing with students.",
                image: "testimonial-avata-04",
                author:"MADLEY PONDOR",
                job:"/IT Specialist"
            },
        ]
    }
}
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';

.titles{
padding:60px 0;
h3{
    color:$tertiary-color;
    font-size:20px;
}
h1{
    color:$violet-color;
    span{
        color:$primary-color;
        font-weight:300;
        }
    }
}

.circle_bar{
    margin-top:80px;
    > div{
        background-color:$tertiary-color;
        width: 10px;
        height:10px;
        border-radius:50%;
        margin:10px;
        }
}

</style>