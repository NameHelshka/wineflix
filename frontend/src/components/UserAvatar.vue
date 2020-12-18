<template>
  <span class="user-avatar">
    <a href="#">{{ username }}</a>
  </span>
</template>

<script>
export default {
  name: 'UserAvatar',
  props: {
    username: String,
  },
};
</script>
