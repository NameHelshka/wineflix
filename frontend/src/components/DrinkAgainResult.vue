<template>
  <li>
    <div class="wine">
      <img src="/red-wine.jpg" alt="Wine">
      <span v-if="isNew" class="new-badge">New!</span>
    </div>
  </li>
</template>

<script>
export default {
  name: 'DrinkAgainResult',
  props: {
    isNew: Boolean,
  },
};
</script>
