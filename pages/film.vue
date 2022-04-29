<template>
<div>
  <navigation></navigation>
  <center><div class="desc">

   
<select v-model="trie" @change="triefilm">
      <option value="classement">classement</option>
      <option value="sortie">date</option>
      <option value="titre">nom</option>
      </select> 
      <input v-model="recherche" @change=triefilm>
   <div v-for="film in films" :key="film.movie">
      <Movie 
     
       :classement=film.classement
       :titre=film.titre
      :image=film.image  
      :link=film.slug 
      :sortie=film.sortie
      ></Movie>
   </div>{{trie}}
     

  </div> 
  </center>
</div>
</template>
<script>
import navigation from '../components/navigation.vue'
import Movie from '../components/movie.vue'
export default {

 async asyncData({$content}){
    const films=await $content('fr').sortBy('sortie').fetch()
    return{films}
 },
 data(){
    return { trie:"classement",recherche:""}
 },
 methods:{
    async triefilm(){
       this.films = await this.$content('fr').search(this.recherche).sortBy(this.trie).fetch()
    }
 },
 name: 'filmPage'
  }
</script>
<style>
body{
   color:white;font-size:30px;
   background-image:url("/etoil.jpg");
   background-attachment: fixed;
   
   
   }
   pre{color:white;}

.desc{margin:30px;text-align: center;  text-shadow:
   -4px -4px 0 #000,  
   -4px -4px 0 #000,  
    4px -4px 0 #000,
    -4px 4px 0 #000,
     4px 4px 0 #000;padding-top: 50px;}
     
</style>