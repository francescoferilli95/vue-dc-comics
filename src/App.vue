<template>
  <div id="app">
    <!-- HEADER -->
    <header>
      <Header />
    </header>
    
    <!-- MAIN CONTENT -->
    <main>
      <Content />
    </main>
    <!-- FOOTER -->
    <footer>
      <Footer />
    </footer>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Content from '@/components/Content.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Content,
    Footer
  }
}
</script>

<style>

  /* GENERAL */

  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  a {
    color: #000;
  }

  .container {
    width: 1500px;
    margin: 0 auto;
  }
</style>
