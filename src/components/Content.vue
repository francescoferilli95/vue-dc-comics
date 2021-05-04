<template>
  <main>
    <div class="content">
        <div class="container">
        <h1>--> Content Goes Here</h1>
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
export default {
    name: 'Content',
}
</script>

<style scoped>
    .content {
        height: 100px;
        background: #0e0e0e;
        color: #fff;
        display: flex;
        align-items: center;
    }
    .shop {
        height: 139px;
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



</style>