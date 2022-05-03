<!-- Please remove this file from your project -->
<template>
 <div>
 <b-navbar toggleable="lg" type="dark" variant="dark"fixed="top">
    <b-navbar-brand href="#"><img src="/star-wars/star wars logo.png"class="logo"></b-navbar-brand>
    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item href="/star-wars/">accueil</b-nav-item>
        <b-nav-item href="/star-wars/film">films et serie</b-nav-item>
      </b-navbar-nav>
    
        </b-nav-item-dropdown>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar> </div>
</template>

<script>
export default {
  name: 'NuxtTutorial'
}
</script>
<style>
.logo{width:100px;}
</style>