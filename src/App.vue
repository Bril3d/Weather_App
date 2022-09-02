<template>
  <div class="bg-weather-primary flex flex-col min-h-screen font-Roboto">
    <SiteNavigation />
    <RouterView v-slot="{ Component }">
      <Transition name="page" mode="out-in">
        <component :is="Component" />
      </Transition>
    </RouterView>
  </div>
</template>

<script setup>
import SiteNavigation from './components/SiteNavigation.vue'
import { RouterView } from "vue-router";
</script>


<style>
  .page-enter-active {
  transition: 600ms ease all;
}
.page-enter-from {
  opacity: 0;
}
</style>