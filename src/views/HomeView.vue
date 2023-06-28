<template>
  <div class="callout-container">
    <h1 class="sr-only">Movie Sites</h1>
  </div>
  
  <div class="wrapper">
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
  </div>
  </template>

<script setup>
import ContactForm from './../components/ContactForm.vue'
import MovieCard from './../components/MovieCard.vue'

</script>

<style scoped>
.introduction {
  margin: 0 80px;
  width: 35%;
  font-size: 1.2em;
  padding-bottom: 20px;
}
.introduction h2 {
  font-size: 2em;
  font-weight: 400;
  text-transform: uppercase;
}
.quick-info{
  background-color: #1D1D1D;
  padding: 25px 75px;
}
.quick-info-search{
  display: flex;
  justify-content: space-between;
  align-items: baseline;
  margin: 0 11px;
}
.quick-info-lookup {
  background: transparent;
  border: 1px solid dimgray;
  margin: 15px 0;
  color: dimgray;
  width: 250px;
  height: 19px;
  padding: 5px;
}

hr{
  padding: 0 20px;
  margin: 0 11px 21px;
}
</style>