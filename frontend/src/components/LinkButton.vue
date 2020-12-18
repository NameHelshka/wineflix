<template>
  <button :class="classname">
    <FontAwesomeIcon :icon="icon" />
    <span>{{ text }}</span>
  </button>
</template>

<script>
export default {
  name: 'AppHeader',
  props: {
    icon: String,
    classname: String,
    text: String,
  },
};
</script>
