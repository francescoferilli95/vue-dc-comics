<template>
  <div id="app">
    <!-- HEADER -->
    <header>
      <Header />
    </header>
    
    <!-- MAIN CONTENT -->
    <main>

    </main>

    <!-- FOOTER -->
    <footer>

    </footer>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'

export default {
  name: 'App',
  components: {
    Header
  }
}
</script>

<style>

  /* GENERAL */
  .container {
    width: 1000px;
    margin: 0 auto;
  }
</style>
