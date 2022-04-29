<template>
 <div>
   {{video}}
  <h1>{{classement}}
  {{titre}}</h1>
  {{sortie}}
  <p>{{description}}</p>
  <nuxt-link :to="'/info/'+link"> 
    <img :src="'/star-wars'+image"/></nuxt-link>
    
 


 </div>
</template>
<script>
export default {
  name: 'Movie',
  props:{
    video:{
      type: String,
      default(){return " "}
    },
    classement:{
      type: String,
      default(){return "-"}
    },
    sortie:{
      type: String,
      default(){return "-"}
    },
    link:{
      type: String,
      default(){return "/info/1"}
    },
    image: {
      type: String,
      default(){ return "/star-wars-1.webp"}
      },
      titre:{type: String,
    default(){return "titre"}
    },
    description:{
      type: String,
      default(){ return " "}
    },
  }
}
</script>
<style>
p{color: white;font-size: 30px;}
img{width:20%;}
h1{color:white}
</style>