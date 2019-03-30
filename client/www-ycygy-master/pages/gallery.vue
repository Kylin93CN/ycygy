<template>
  <section class="container">
    <div>
      <Header />
      <Container />
      <Footer />
    </div>
  </section>
</template>

<script>
import Header from '~/components/common/Header.vue';
import Container from '~/components/gallery/Container.vue';
import Footer from '~/components/common/Footer.vue';
export default {
  components: {
    Header,
    Container,
    Footer
  }
}
</script>
<style>
body, div, dl, dt, dd, ul, ol, li, h1, h2, h3, h4, h5, h6, pre, code, form, fieldset, legend, input, button, textarea, p, blockquote, table, th, td  {
  margin: 0;
  padding: 0;
}
</style>

