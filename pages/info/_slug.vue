<template>
    <div>
       
   <navigation></navigation>

    <br/>
    <center>
    <p>{{film.titre}}</p>

        {{film.classement}}
    <img :src="film.image" />
    <div class=descr><p>{{film.description}}</p></div>
        {{film.sortie}}

      <iframe width="560" height="315" :src="film.video" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      
    </center>
    </div>
</template>

<script>
import navigation from '../../components/navigation.vue'
export default {
  components: { navigation },
  name: 'Info',
   async asyncData({ params,$content}) {
        const film=await $content('fr/'+params.slug).fetch()

       return {slug: params.slug,film}
   }
}
</script>
<style>
body{
   color:rgb(255, 255, 255);font-size:30px;
   background-image:url("/etoil.jpg");
   background-attachment: fixed;
font-family : 'Tapestry', cursive ;
   }
pre{color:rgb(255, 255, 255);margin:30px;text-align: center;  text-shadow:
   -2px -2px 0 #000,  
   -2px -2px 0 #000,  
    2px -2px 0 #000,
    -2px 2px 0 #000,
     2px 2px 0 #000;;}
.descr{width:50%;}
</style>