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

            <!--TITLESBOTTOM-->
            <div class="titles_bottom text-center">
                <h3>Start today for getting <span>Online Certification</span></h3>
                <h1>You can be your own guiding star with our help!</h1>
                <button class="button">Get started now</button>

            <!--DETAILS-->
                <img class="circle" src="../assets/maxcoach-shape-02.png" alt="circle">
                <img class="stripes" src="../assets/maxcoach-shape-01.png" alt="stripes">
                <i class="far fa-circle"></i>
                
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

section{
    background-color:#f8f8f8;
}

/*TITLES*/
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

/*CIRCLE BAR*/
.circle_bar{
    padding:80px 0;
    > div{
        background-color:$tertiary-color;
        width: 10px;
        height:10px;
        border-radius:50%;
        margin:10px;
        &:hover {
        background-color:$violet-color;
        width:15px;
        height:15px;
        cursor: pointer;
        }
        }
}

/*TITLES*/
.titles_bottom{
padding:50px 0;
position:relative;

/*DETAILS*/
.circle{
    position:absolute;
    right:20px;
}
.stripes{
    position:absolute;
    left:6px;
}
.fa-circle{
        position:absolute;
        left:0;
        bottom:220px;
        color:#efcfba;
        font-size:60px;
    }
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
button{
    margin:60px 0;
}
}

</style>