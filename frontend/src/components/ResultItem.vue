<template>
    <div class="wine">
      <img src="/red-wine.jpg" alt="Wine">
      <span class="new-badge">New!</span>
    </div>
</template>

<script>
export default {
  name: 'ResultItem',
  props: {
    msg: String,
  },
};
</script>
