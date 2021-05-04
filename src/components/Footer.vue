<template>
  <footer>
    <div class="container">
    <div class="main-footer">
              <div class="footer-nav">
        <ul>
          <h3>DC Comics</h3>
          <li v-for="(link, index) in links1" :key="index">
            <a :href="link.url">{{ link.text }}</a>
          </li>
        </ul>
        <ul>
          <h3>DC</h3>
          <li v-for="(link, index) in links2" :key="index">
            <a :href="link.url">{{ link.text }}</a>
          </li>
        </ul>
        <ul>
          <h3>SITES</h3>
          <li v-for="(link, index) in links3" :key="index">
            <a :href="link.url">{{ link.text }}</a>
          </li>
        </ul>
        <ul>
          <h3>SHOP</h3>
          <li v-for="(link, index) in links4" :key="index">
            <a :href="link.url">{{ link.text }}</a>
          </li>
        </ul>
      </div>
      <div class="footer-logo">
        <img src="../assets/img/dc-logo-bg.png" alt="" />
      </div>
    </div>
    </div>
    <div class="footer-social">
      <div class="sign">
        <button>Sign Up Now!</button>
      </div>
      <div class="follow">
        <span>FOLLOW US</span>
        <img
          src="../assets/img/footer-facebook.png"
          alt="Footer Facebook Social"
        />
        <img
          src="../assets/img/footer-twitter.png"
          alt="Footer Twitter Social"
        />
        <img
          src="../assets/img/footer-youtube.png"
          alt="Footer Youtube Social"
        />
        <img
          src="../assets/img/footer-pinterest.png"
          alt="Footer Pinterest Social"
        />
        <img
          src="../assets/img/footer-periscope.png"
          alt="Footer Periscope Social"
        />
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      links1: [
        { text: "Characters", url: "/" },
        { text: "Comics", url: "/" },
        { text: "Movies", url: "/" },
        { text: "TV", url: "/" },
        { text: "Games", url: "/" },
        { text: "Videos", url: "/" },
        { text: "News", url: "/" },
      ],
      links2: [
        { text: "Terms Of Use", url: "/" },
        { text: "Privacy policy(New)", url: "/" },
        { text: "Ad Choices", url: "/" },
        { text: "Advertising", url: "/" },
        { text: "Jobs", url: "/" },
        { text: "Subscriptions", url: "/" },
        { text: "Talent Workshops", url: "/" },
        { text: "CPSC Certificates", url: "/" },
        { text: "Ratings", url: "/" },
        { text: "Shop Help", url: "/" },
        { text: "Contact Us", url: "/" },
      ],
      links3: [
        { text: "DC", url: "/" },
        { text: "MAD Magazine", url: "/" },
        { text: "DC Kids", url: "/" },
        { text: "DC Universe", url: "/" },
        { text: "DC Power Visa", url: "/" },
      ],
      links4: [
        { text: "Shop DC", url: "/" },
        { text: "Shop DC Collectibles", url: "/" },
      ],
    };
  },
};
</script>

<style scoped>
footer {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    background-image: url(/img/footer-bg.dfd68d29.jpg);
    height: 600px;
}

.container {
    position: relative;
}

ul li {
  list-style: none;
  padding: .3rem 1rem;
}

ul {
    margin: 1rem;
}

h3 {
    color: #fff;
    padding-left: 15px;
}

a {
  text-decoration: none;
  color: #959595;
}

.footer-nav {
  display: flex;
  padding: 2rem;
}



.footer-logo {
    position: absolute;
    top: 0;
    right: 0;
}

.footer-social {
    height: 100px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: #303030;
    z-index: 1;
}

.sign {
    display: flex;
    align-items: center;
    padding-left: 202px;
}

.footer-social button {
    width: 250px;
    padding: 5px;
    border: 2px solid #0282f9;
    background: transparent;
    color: #fff;
    cursor: pointer;
}

.follow {
    display: flex;
    align-items: center;
    padding-right: 202px;
}

.footer-social span {
    color: #0282f9;
}

.main-footer {
    display: flex;
    height:400px;
}

</style>