<template>

  <div class="card">
      <!--CARD-->
      <h3>{{title}}</h3>
      <p>{{text}}</p>
        
      <!--DETAILS-->
      <div class=" d-flex">
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

.card{
  background-color:white;
  padding:30px;
  transition:0.5 ease;
  &:hover {
    transform:scale(1.2);
    cursor:pointer;
    z-index:1;
    box-shadow: 0 0 11px rgba(33,33,33,.2); 
  }
}
h3{
color:$violet-color;
font-size:20px;
}
p{
  color:$tertiary-color;
  padding:20px 0;
}
img{
  border-radius:50%;
  width:100px;
  height:100px;
}

.details{
  padding-left:20px;

}
</style>