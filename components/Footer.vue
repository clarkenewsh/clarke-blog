<template>
  <footer>
    <nuxt-link to="/">
      Home
    </nuxt-link>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
  props: {
    // eslint-disable-next-line vue/require-default-prop
    msg: String
  }
}

</script>
<style>
footer {
    height: 8rem;
    border-top: 5px solid lightseagreen;
    width: 100%;
}
</style>
