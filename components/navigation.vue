<!-- Please remove this file from your project -->
<template>
 <div>
 <b-navbar toggleable="lg" type="dark" variant="dark"fixed="top">
    <b-navbar-brand href="#"><img src="/star-wars/star wars logo.png"class="logo"></b-navbar-brand>
    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item href="/star-wars/">accueil</b-nav-item>
        <b-nav-item href="/star-wars/film">films</b-nav-item>
      </b-navbar-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-nav-form>
          <b-form-input size="sm" class="mr-sm-2" placeholder="recherche"></b-form-input>
          <b-button size="sm" class="my-2 my-sm-0" type="submit">Search</b-button>
        </b-nav-form>

        <b-nav-item-dropdown text="lang" right>
          <b-dropdown-item href="#">englais</b-dropdown-item>
          <b-dropdown-item href="#">français</b-dropdown-item>
        </b-nav-item-dropdown>

        
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