<template>
  <Header></Header>
  <main>
    <ProjectsInfo></ProjectsInfo>
    <Request></Request>
  </main>
  <Footer></Footer>
</template>

<script>
import Header from './components/Header.vue'
import ProjectsInfo from './components/ProjectsInfo.vue'
import Request from './components/Request.vue'
import Footer from './components/Footer.vue'

export default {
  components: {
    Header,
    ProjectsInfo,
    Request,
    Footer
  }
}

</script>

<style></style>
