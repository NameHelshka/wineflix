<template>
  <section class="category">
    <h2>{{ header_text }}</h2>
    <ul class="category-links">
      <li
        v-for="wine in data_list"
        :key = "wine.id"
      >
        <DrinkAgainResult
          :isNew="wine.isNew"
        />
      </li>
    </ul>
  </section>
</template>

<script>
import DrinkAgainResult from '@/components/DrinkAgainResult';

export default {
  name: 'DrinkAgainSection',
  components: {
    DrinkAgainResult,
  },
  props: {
    header_text: String,
    data_list: Object,
  },
};
</script>
