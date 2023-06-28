<template>
  <div class="card">
    <img v-bind:src="image" alt="Movie still">
    <div class="card-body">
      <div class="card-title">
        {{ title }}
      </div>
      <div class="card-desc">
        Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut...
      </div>
    </div>
    
    <button class="card-delete-btn">
      &times;
    </button>
  </div>
</template>

<script setup>
  // eslint-disable-next-line no-unused-vars
  const props = defineProps({
    title: {
      type: String,
      default: 'Could not find title'
    },
    image: {
      type: String
    }
  })
</script>