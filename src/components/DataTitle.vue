<template>
  <div class="text-center">
    <h2 class="text-3xl font-bold">{{ text }}</h2>
    <div class="text-2xl mt-4 mb-10">
      {{ timestamp }}
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import moment from "moment";

export default defineComponent({
  name: "DataTitle",
  props: {
    text: String,
    dataDate: String,
  },
  computed: {
    timestamp: function () {
      return moment(this.dataDate).format("MMMM Do YYYY, h:mm a");
    },
  },
});
</script>
