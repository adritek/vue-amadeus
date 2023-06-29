<template>
  <div class="callout-container">
    <h1 class="sr-only">Movie Sites</h1>
  </div>
  
  <div class="introduction">
    <h2>Movie Library</h2>
    <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.</p>
  </div>

  <div class="quick-info">
    <div class="quick-info-search">
      <h2>Collect your favourites</h2>
      <input class="quick-info-lookup" type="text" placeholder="🔍 Search title an add to grid">
    </div>

    <hr class="hr-white">
    
    <div class="card-container">
      <MovieCard title="Batman Returns" image="/images/batman.jpg" />
      <MovieCard title="Wild Wild West" image="/images/wild-west.jpg" />
      <MovieCard title="The Amazing Spiderman" image="/images/spiderman.jpg" />
    </div>
  </div>

  <ContactForm />
</template>

<script setup>
  import ContactForm from './../components/ContactForm.vue'
  import MovieCard from './../components/MovieCard.vue' 
</script>