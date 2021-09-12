<template>
  <Header />
  <div class="container">
    <router-view />
  </div>
</template>

<script>
import { defineComponent } from "vue";
import Header from "@/components/Header";

export default defineComponent({
  components: {
    Header,
  },
});
</script>
