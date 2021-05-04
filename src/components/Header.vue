<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="DC LOGO HEADER">
            </div>
            <nav class="navigation">
                <ul>
                    <li><a href="/">Characters</a></li>
                    <li><a href="/">Characters</a></li>
                    <li><a href="/">Characters</a></li>
                    <li><a href="/">Characters</a></li>
                    <li><a href="/">Characters</a></li>
                    <li><a href="/">Characters</a></li>
                    <li><a href="/">Characters</a></li>
                    <li><a href="/">Characters</a></li>
                    <li><a href="/">Characters</a></li>
                    <li><a href="/">Characters</a></li>

                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: 'Header',
}
</script>

<style scoped>
.container {
    display: flex;
    justify-content: space-between;
}

.navigation ul {
    display: flex;
    list-style: none;
}

ul a {
    padding: 1rem;
    text-decoration: none;
    color: #000;
}
</style>