<template>
  <div class="grid">
    <header>
      <Nav />
    </header>
    <main>
      <Nuxt />
    </main>
    <Footer />
  </div>
</template>

<script>
import Nav from '~/components/NavBar.vue'
import Footer from '~/components/Footer.vue'
export default {
  components: {
    Nav,
    Footer
  }
}
</script>

<style>

html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  color: #2E495E;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.grid {
  display: grid;
  grid-template-columns: 1% 1fr 1%;
  grid-column-gap: 1rem;
  grid-row-gap: 3rem;
}

main {
  min-height: 100vh;
}

header, main, footer {
  grid-column: 2;
}

footer {

}

@media only screen and (min-width: 768px) {
  .grid {
    grid-template-columns: 3% 1fr 3%;
  }
}

@media only screen and (min-width: 1024px) {
    .grid {
      grid-template-columns: 6% 1fr 6%;
  }
 }

@media only screen and (min-width: 1400px) {
      .grid {
      grid-template-columns: 15% 1fr 15%;
  }
}
</style>
