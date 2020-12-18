<template>
  <a
  :href="url"
  >{{ label }}
  </a>
</template>

<script>
export default {
  name: 'NavigationLink',
  props: {
    label: String,
    url: String,
    isActive: Boolean,
  },
};
</script>
