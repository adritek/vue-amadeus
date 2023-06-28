<template>
  <aside class="sidebar-menu-container" id="sbm1">
      <div class="sidebar-menu">
        <h1 class="sidebar-menu-title">
          <span>
            More options menu
          </span>
          <button class="sidebar-menu-close" @click="$emit('hideSideBarMenu')" aria-controls="sbm1">&times;</button>
        </h1>
        <hr />
        <ul class="sidebar-menu-ul" role="menu">
          <li class="sidebar-menu-li" role="menuitem" tabindex="0">Popcorn</li>
          <li class="sidebar-menu-li" role="menuitem" tabindex="0">Tickets</li>
          <li class="sidebar-menu-li" role="menuitem" tabindex="0">Drinks</li>
          <li class="sidebar-menu-li" role="menuitem" tabindex="0">Parking</li>
          <li class="sidebar-menu-li" role="menuitem" tabindex="0">Donuts</li>
        </ul>
      </div>
    </aside>
</template>

<script setup>
  // eslint-disable-next-line no-unused-vars
  const emit = defineEmits(['hideSideBarMenu'])

</script>