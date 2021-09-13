<template>
  <select
    @change="onChange()"
    v-model="selected"
    class="form-select block w-full border p-3 rounded mt-10"
  >
    <option value="0">Select a Country</option>
    <option v-for="country in countries" :key="country.ID" :value="country.ID">
      {{ country.Country }}
    </option>
  </select>
</template>

<script lang="ts">
import { defineComponent, PropType } from "vue";

export default defineComponent({
  name: "CountrySelect",
  props: {
    countries: Array as PropType<any[]>,
  },
  data() {
    return {
      selected: 0,
    };
  },
  methods: {
    onChange() {
      const country = this.countries?.find((c) => c.ID === this.selected);
      this.$emit("get-country", country);
    },
  },
});
</script>
