<template>
  <div>
      <!--CARD-->
      <h3>{{title}}</h3>
        <p>{{text}}</p>
        
        <!--DETAILS-->
        <div class="d-flex">
        <img :src="require(`../assets/${image}.jpg`)" :alt="title">

        <div class="details">
        <span>{{subtext}}</span>
        <p>{{subtextTwo}}</p>
        </div>

        </div>
      </div>

</template>

<script>
export default {
name:'Card',
props:{
  title:String,
  text:String,
  image:String,
  subtext:String,
  subtextTwo:String,
}
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';

h3{
color:$violet-color;
}
p{
  color:$tertiary-color;
  padding:20px 0;
}
img{
  border-radius:50%;
  width:100px;
}

.details{
  padding-left:20px;
}
</style>