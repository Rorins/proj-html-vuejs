<template>
  <div id="app">
  <!--HEADER-->
  <Header />

  <!--JUMBO-->
  <Jumbo />

  <!--MAIN-->
  <main>
  <SectionOne />
  <SectionTwo />
  <SectionThree />
  </main>

  </div>
</template>

<script>
//IMPORTS
import Header from '@/components/Header.vue';
import Jumbo from '@/components/Jumbo.vue';
import SectionOne from '@/components/SectionOne.vue';
import SectionTwo from '@/components/SectionTwo.vue';
import SectionThree from '@/components/SectionThree.vue';

export default {
  name: 'App',
  components: {
    Header,
    Jumbo,
    SectionOne,
    SectionTwo,
    SectionThree,
  }
}
</script>

<style lang="scss">
@import '@/styles/globals';
@import '@/styles/utilities';
</style>
