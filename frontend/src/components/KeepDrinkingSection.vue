<template>
  <section class="category">
    <h2>{{ header_text }}</h2>
    <ul class="category-links">
      <li
        v-for="wine in data_list"
        :key = "wine.id"
      >
        <KeepDrinkingResult
          :progress="wine.progress"
        />
      </li>
    </ul>
  </section>
</template>

<script>
import KeepDrinkingResult from "@/components/KeepDrinkingResult";

export default {
  name: 'KeepDrinkingSection',
  components: {
    KeepDrinkingResult,
  },
  props: {
    header_text: String,
    data_list: Object,
  },

};
</script>
