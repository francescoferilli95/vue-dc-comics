<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="DC LOGO HEADER">
            </div>
            <nav class="navigation">
                <ul>
                    <li v-for="(link, index) in links" :key="index"><a :href="link.url" :class="{active: link.current}">{{link.text}}</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            links: [
                {text: 'Characters', url: '/Characters', current: false},
                {text: 'Comics', url: '/Comics', current: true},
                {text: 'Movies', url: '/Movies', current: false},
                {text: 'TV', url: '/TV', current: false},
                {text: 'Games', url: '/Games', current: false},
                {text: 'Collectibles', url: '/Collectibles', current: false},
                {text: 'Videos', url: '/Videos', current: false},
                {text: 'Fans', url: '/Fans', current: false},
                {text: 'News', url: '/News', current: false},
                {text: 'Shop', url: '/Shop', current: false},
            ],
        }
    },
}
</script>

<style scoped lang="scss">
header {
    padding: 1rem 0;
}

.container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo img {
    width: 60%;
    cursor: pointer;
}

.navigation ul {
    display: flex;
    align-items: center;
    list-style: none;
}

ul a {
    padding: .5rem;
    text-decoration: none;
    text-transform: uppercase;
    transition: background .3s;
}

.active {
    color: dodgerblue;
}

ul a:hover {
    background: dodgerblue;
}

ul li:nth-child(2) a:hover {
    color: #fff;
}

</style>