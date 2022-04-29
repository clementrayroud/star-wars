<template>
<div>
    <navigation></navigation>

  <p id="start">A short time ago in a browser very, very close&hellip;</p>

<h1>STAR WARS<sub>titles in CSS3</sub></h1>

<div id="titles">
  <div id="titlecontent">

<h1>sta wars</h1>
 <center><div class="par"><p>
   Un saigneur sith apparait après des décennies de paix. 
   Des millions de cloneps sont créés pour poursuivre la guerre. 
   Le saigneur Sidious  retourne les clones contre les jeudi et gagne la guerre puis il instaure 
   une dictature.</p><p> Une alliance rebelle est créée pour rétablir la paix dans la galaxie. l’étoile de la mort explose et l’empire se sépare.</p><p>
La nouvelle république est créée et Leila organa est critiqué, car sont père était dark wador elle a toujours dit qu’il ne fallait pas supprimé une grosse partie de l’armé, car l’empire reviendra. Elle C’est réfugié en recréent la résistance, le premier ordre renverse la démocratie grasse au nombreux cuirassé et a la basse starkilleur. La résistance re rend sur la planète cachée des sites pour tué palpatine et détruire le premier ordre
</p><p>fait par Clément Rayroud</p></div>
   </center>
  </div></div></div>
</template>
<script>
import navigation from '../components/navigation.vue'
export default {
  components: { navigation },
  name: 'IndexPage'
}
</script>
<style>

h1{color:red;text-align: center;}
p{color:gold;font-size: 60px;}
body{background-image:url("/star-wars/etoil.jpg");background-attachment: fixed;  font-family: "Droid Sans", arial, verdana, sans-serif;
	font-weight: 700;}

.par p{margin:30px;text-align: justify;  text-shadow:
   -2px -2px 0 #000,  
   -2px -2px 0 #000,  
    2px -2px 0 #000,
    -2px 2px 0 #000,
     2px 2px 0 #000;;}

@import url(https://fonts.googleapis.com/css?family=Droid+Sans:400,700);

p#start
{
	position: relative;
	width: 16em;
	font-size: 200%;
	font-weight: 400;
	margin: 20% auto;
	color: #4ee;
	opacity: 0;
	z-index: 1;
	-webkit-animation: intro 2s ease-out;
	-moz-animation: intro 2s ease-out;
	-ms-animation: intro 2s ease-out;
	-o-animation: intro 2s ease-out;
	animation: intro 2s ease-out;
}

@-webkit-keyframes intro {
	0% { opacity: 1; }
	90% { opacity: 1; }
	100% { opacity: 0; }
}

@-moz-keyframes intro {
	0% { opacity: 1; }
	90% { opacity: 1; }
	100% { opacity: 0; }
}

@-ms-keyframes intro {
	0% { opacity: 1; }
	90% { opacity: 1; }
	100% { opacity: 0; }
}

@-o-keyframes intro {
	0% { opacity: 1; }
	90% { opacity: 1; }
	100% { opacity: 0; }
}

@keyframes intro {
	0% { opacity: 1; }
	90% { opacity: 1; }
	100% { opacity: 0; }
}

h1
{
	position: absolute;
	width: 2.6em;
	left: 50%;
	top: 25%;
	font-size: 10em;
	text-align: center;
	margin-left: -1.3em;
	line-height: 0.8em;
	letter-spacing: -0.05em;
	color: #000;
	text-shadow: -2px -2px 0 #ff6, 2px -2px 0 #ff6, -2px 2px 0 #ff6, 2px 2px 0 #ff6;
	opacity: 0;
	z-index: 1;
	-webkit-animation: logo 5s ease-out 2.5s;
	-moz-animation: logo 5s ease-out 2.5s;
	-ms-animation: logo 5s ease-out 2.5s;
	-o-animation: logo 5s ease-out 2.5s;
	animation: logo 5s ease-out 2.5s;
}

h1 sub
{
	display: block;
	font-size: 0.3em;
	letter-spacing: 0;
	line-height: 0.8em;
}


@keyframes logo {
	0% { transform: scale(1); opacity: 1; }
	50% { opacity: 1; }
	100% { transform: scale(0.1); opacity: 0; }
}

/* the interesting 3D scrolling stuff */
#titles
{
	position: absolute;
	width: 18em;
	height: 50em;
	bottom: 0;
	left: 50%;
	margin-left: -9em;
	font-size: 350%;
	text-align: justify;
	overflow: hidden;
	-webkit-transform-origin: 50% 100%;
	-moz-transform-origin: 50% 100%;
	-ms-transform-origin: 50% 100%;
	-o-transform-origin: 50% 100%;
	transform-origin: 50% 100%;
	-webkit-transform: perspective(300px) rotateX(25deg);
	-moz-transform: perspective(300px) rotateX(25deg);
	-ms-transform: perspective(300px) rotateX(25deg);
	-o-transform: perspective(300px) rotateX(25deg);
	transform: perspective(300px) rotateX(25deg);
}

#titles:after
{
	position: absolute;
	content: ' ';
	left: 0;
	right: 0;
	top: 0;
	bottom: 60%;
	background-image: -webkit-linear-gradient(top, rgba(0,0,0,1) 0%, transparent 100%);
	background-image: -moz-linear-gradient(top, rgba(0,0,0,1) 0%, transparent 100%);
	background-image: -ms-linear-gradient(top, rgba(0,0,0,1) 0%, transparent 100%);
	background-image: -o-linear-gradient(top, rgba(0,0,0,1) 0%, transparent 100%);
	background-image: linear-gradient(top, rgba(0,0,0,1) 0%, transparent 100%);
	pointer-events: none;
}

#titles p
{
	text-align: justify;
	margin: 0.8em 0;
}

#titles p.center
{
	text-align: center;
}

#titles a
{
	color: #ff6;
	text-decoration: underline;
}

#titlecontent
{
	position: absolute;
	top: 100%;

	animation: scroll 200s linear 4s infinite;
}

/* animation */
@-webkit-keyframes scroll {
	0% { top: 100%; }
	100% { top: -170%; }
}

@-moz-keyframes scroll {
	0% { top: 100%; }
	100% { top: -170%; }
}

@-ms-keyframes scroll {
	0% { top: 100%; }
	100% { top: -170%; }
}

@-o-keyframes scroll {
	0% { top: 100%; }
	100% { top: -170%; }
}

@keyframes scroll {
	0% { top: 100%; }
	100% { top: -170%; }
}


</style>