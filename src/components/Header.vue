<template>
  <header class="text-center bg-blue-600 text-white p-4 mb-10">
    <div class="text-3xl md:text-5xl fond-bold mb-3">
      <i class="fa fa-viruses"></i> COVID-19 Tracker
    </div>
    <p>
      API by
      <a class="text-blue-300" href="https://covid19api.com" target="_blank"
        >covid19api.com</a
      >
    </p>
  </header>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Header",
});
</script>
