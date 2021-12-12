<template>
  <div id="app">
  <!--HEADER-->
  <Header :links="links" />

  <!--JUMBO-->
  <Jumbo />

  <!--MAIN-->
  <main>
  <SectionOne />
  <SectionTwo />
  <SectionThree />
  <SectionFour />
  <SectionFive />
  <SectionSix />
  </main>

  <!--FOOTER-->
  <Footer :exploreLinks="exploreLinks" :informationLinks="informationLinks"/>
  </div>
</template>

<script>
//IMPORTS
import Header from '@/components/Header.vue';
import Jumbo from '@/components/Jumbo.vue';
import SectionOne from '@/components/SectionOne.vue';
import SectionTwo from '@/components/SectionTwo.vue';
import SectionThree from '@/components/SectionThree.vue';
import SectionFour from '@/components/SectionFour.vue';
import SectionFive from '@/components/SectionFive.vue';
import SectionSix from '@/components/SectionSix.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Jumbo,
    SectionOne,
    SectionTwo,
    SectionThree,
    SectionFour,
    SectionFive,
    SectionSix,
    Footer,
  },
  //LINKS ARRAY
  data(){
  return{
    links:[
      "Home",
      "Pages",
      "Courses",
      "Features",
      "Blog",
      "Shop"
    ],
    exploreLinks:[
      "Start here ",
      "Blog",
      "About us",
      "Success story",
      "Courses",
      "Contact us",
    ],
    informationLinks:[
      "Membership",
      "Purchase guide",
      "Privacy Policy",
      "Terms of services"
    ],
  
  }
}
}
</script>

<style lang="scss">
//SASS IMPORTS
@import '@/styles/globals';
@import '@/styles/utilities';
</style>
