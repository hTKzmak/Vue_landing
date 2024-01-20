<template>
  <Header></Header>
  <main>
    <SecondPart></SecondPart>
    <Banner></Banner>
  </main>
  <Footer></Footer>
</template>

<script>
import Header from './components/Header.vue'
import SecondPart from './components/SecondPart.vue'
import Banner from './components/Banner.vue'
import Footer from './components/Footer.vue'

export default {
  components: {
    Header,
    SecondPart,
    Banner,
    Footer
  }
}

</script>

<style></style>
