<template>
  <header class="top-bar">
    <img alt="Amadeus Logo" class="logo" src="@/assets/logo-white.svg" width="125" height="125" />
    <nav class="top-bar-nav">
      <RouterLink to="/" class="top-bar-link"><span>Home</span></RouterLink>
      <RouterLink to="/our-screens" class="top-bar-link"><span>Our Screens</span></RouterLink>
      <RouterLink to="/schedule" class="top-bar-link"><span>Schedule</span></RouterLink>
      <RouterLink to="/movie-library" class="top-bar-link"><span>Movie Library</span></RouterLink>
      <RouterLink to="/location-contact" class="top-bar-link"><span>Location & Contact</span></RouterLink>
      <a @click="showSidebarMenu = true" tabindex="0" role="button">
        <img src="@/assets/menu-white.svg" alt="Menu" width="25" height="25">
      </a>
    </nav>
    <SidebarMenu 
      v-if="showSidebarMenu"
      @hideSideBarMenu="showSidebarMenu = false"
    />
  </header>
  <RouterView />
</template>

<script setup>
import { ref } from 'vue'
import { RouterLink, RouterView } from 'vue-router'
import SidebarMenu from './components/SidebarMenu.vue'

const showSidebarMenu = ref(false)
</script>