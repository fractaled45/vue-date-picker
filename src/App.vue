<template>
  <h1 class="font-large">Test</h1>
  <div class="m-32 border">
    <EpicCalendar />
  </div>

  <RouterView />
</template>

<script setup lang="ts">
import { RouterView } from "vue-router";
import EpicCalendar from "./components/EpicCalendar.vue";
</script>
