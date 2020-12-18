<template>
  <div class="wine">
    <img src="/red-wine.jpg" alt="Wine">
    <div class="amount-consumed">
      <progress min="0" max="100" :value="progress"></progress>
    </div>
  </div>
</template>

<script>
export default {
  name: 'KeepDrinkingResult',
  props: {
    progress: Number,
  },
};
</script>
