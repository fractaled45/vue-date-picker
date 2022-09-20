<template>
  <p class="text-center mb-2">{{ months[8] }} {{ year }}</p>
  <table class="m-auto">
    <thead>
      <tr>
        <td v-for="day in days" :key="day" class="p-2 text-center">
          {{ day }}
        </td>
      </tr>
      <tr v-for="i in 4" :key="i">
        <td
          class="p-2 text-center hover:bg-blue-300 cursor-pointer"
          :class="{ 'border background-blue': false }"
          v-for="j in 7"
          :key="j"
        >
          {{ (i - 1) * 7 + j }}
        </td>
      </tr>
    </thead>
  </table>
</template>

<script setup lang="ts">
import { ref } from "vue";

let days = ref(["M", "T", "W", "T", "F", "S", "S"]);
let months = ref([
  "January",
  "February",
  "March",
  "April",
  "May",
  "June",
  "July",
  "August",
  "September",
  "October",
  "November",
  "December",
]);
let year = ref(2022);
// let selected = ref<Date>(Date.now());
</script>
