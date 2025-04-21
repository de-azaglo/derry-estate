<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import CallToActionButton from './components/CallToActionButton.vue';
import HomeView from './views/HomeView.vue';
import ServiceView from './views/ServiceView.vue';
import SearchView from './views/SearchView.vue';

</script>

<template>
  <header>
    <div class="logo-container">
      <img alt="Vue logo" class="logo" src="@/assets/pictures/logo.png" width="125" height="125" />
      <h3 class="logo-caption">Derry Estate</h3>
    </div>
      <nav>
        <RouterLink to="/">Brands</RouterLink>
        <RouterLink to="/services">Service</RouterLink>
        <RouterLink to="/about">Features</RouterLink>
        <RouterLink to="/about">Contact</RouterLink>
      </nav>
    <CallToActionButton>
      <template #title>Contact Us</template>
    </CallToActionButton>
  </header>

  <HomeView />

  <ServiceView />

  <SearchView />
  <!-- <RouterView /> -->
</template>

<style scoped>
header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-top: 2vh;
  width: 100%;
  padding: 0 5vw;
  /* position: fixed; */
}

.logo-container{
  display: flex;
  align-items: center;
}

.logo-caption{
  margin-left: 8px;
  font-weight: 600;
  color: #fff;
}

.logo {
  width: 2vw;
  height: 2vw;
}

nav {
  font-size: 12px;
  text-align: center;
}

nav a.router-link-exact-active {
  color: #fff;
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  font-size: 1.2em;
  color: rgba(235, 235, 235, 0.64);;
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
 
}
</style>
