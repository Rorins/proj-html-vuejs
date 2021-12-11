<template>
  <div>
    
      <h3>{{title}}</h3>
        <p>{{text}}</p>
        <img :src="require(`../assets/${image}.jpg`)" :alt="title">
      </div>

</template>

<script>
export default {
name:'Card',
props:{
  title:String,
  text:String,
  image:String,
}
}
</script>

<style>

</style>