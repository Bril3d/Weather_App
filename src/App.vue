<template>
  <div class="bg-weather-primary flex flex-col min-h-screen font-Roboto">
    <SiteNavigation />
    <RouterView />
  </div>
</template>

<script setup>
import SiteNavigation from './components/SiteNavigation.vue'
import { RouterView } from "vue-router";
</script>

