<template>
<nav class="navigation">
      <section class="primary-navigation">
        <h1>WineFlix</h1>
        <ul class="navigation-links">
          <li class="active">
            <a href="#">Home</a>
          </li>
          <li>
            <a href="#">Whites</a>
          </li>
          <li><a href="#">Reds</a>
          </li>
          <li><a href="#">Blends</a></li>
        </ul>
      </section>

    </nav>
</template>

<script>
export default {
  name: 'AppHeader',
  props: {
    msg: String,
  },
};
</script>
