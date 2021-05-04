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
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    color: #000;
  }

  .container {
    width: 1500px;
    margin: 0 auto;
  }
</style>
