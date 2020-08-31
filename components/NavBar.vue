<template>
  <nav class="nav">
    <div class="nav__link">
      <nuxt-link to="/">
        Home
      </nuxt-link>
    </div>
    <div class="nav__link">
      <nuxt-link to="/About">
        About
      </nuxt-link>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Nav',
  props: {
    // eslint-disable-next-line vue/require-default-prop
    msg: String
  }
}
</script>
<style>
.nav {
    display: flex;
}

.nav__link {
    padding: 1rem;
}
</style>
