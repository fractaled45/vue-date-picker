<template>
  <h1 class="text-center text-4xl">EPIC CALENDAR!!!</h1>
  <div class="m-32 border">
    <EpicCalendar class="my-4" />
  </div>
</template>

<script setup lang="ts">
import { RouterView } from "vue-router";
import EpicCalendar from "./components/EpicCalendar.vue";
</script>
