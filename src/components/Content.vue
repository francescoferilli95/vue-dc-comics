<template>
  <main>
      <div class="hero">
          <img src="../assets/img/jumbotron.jpg" alt="Jumbotron image Teen Titans">
      </div>
    <div class="content">
        <div class="container">
        <h2>Current Series</h2>
            <Comics v-for="(comic, index) in comics" :key="index" :details="comic" />
            <button>Load More</button>
        </div>
    </div>
    <div class="shop">
        <div class="container">
            <img src="../assets/img/buy-comics-digital-comics.png" alt="Digital Comics">
            <span>Digital Comics</span>
            <img src="../assets/img/buy-comics-merchandise.png" alt="DC Merchandise">
            <span>DC Merchandise</span>
            <img src="../assets/img/buy-comics-subscriptions.png" alt="Subscriptions">
            <span>Subscriptions</span>
            <img src="../assets/img/buy-comics-shop-locator.png" alt="Comic Shop Locator">
            <span>Comic Shop Locator</span>
            <img class="visa" src="../assets/img/buy-dc-power-visa.svg" alt="DC Power Visa">
            <span>DC Power Visa</span>
        </div>
    </div>
  </main>
</template>

<script>
import Comics from '@/components/Comics.vue';
import comicData from '@/data/comicData.js'
export default {
    name: 'Content',
    components: {
        Comics
    },
    data() {
        return {
            comics: comicData
        }
 
    }
}
</script>

<style scoped lang="scss">
    .content {
        padding-top: 50px;
        position: relative;
        background: #0e0e0e;
        color: #fff;
        display: flex;
        align-items: center;
    }

    .content .container {
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
    }

    .shop {
        background: #0282f9;
        color: #fff;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .shop .container {
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .visa {
        width: 50px;
    }

    .shop img {
        width: 7%;
        padding: 0 1rem;

    }

    .content h2 {
        position: absolute;
        top: -28px;
        left: 250px;
        width: 240px;
        padding: 15px;
        text-transform: uppercase;
        background: #0282f9;
    }

    .container button {
        text-align: center;
        text-transform: uppercase;
        background: #0282f9;
        color: #fff;
        border: 0;
        width: 200px;
        padding: 10px;
        margin: 20px 0;
        cursor: pointer;
        transition: scale .3s;
    }

    .container button:hover {
        transform: scale(1.2);
    }

    .hero {
        height: 400px;
        z-index: -1;
        position: relative;
    }

    .hero img {
        width: 100%;
        position: absolute;
    }

</style>