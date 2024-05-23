<script>
export default {
    data() {
        return {
            links: ["Characters", "Comics", "Movies", "TV", "Characters", "Games", "Collectibles", "Videos", "Fans", "News", "Shop"]
        }
    }
}
</script>

<template>
    <header>
        <a v-for="link in links" :href="'#' + link.toLowerCase().replace(/ /g, '')">{{ link }}</a>
    </header>
</template>

<style scoped>
header {
    background: #444;
    padding: 1rem;
}
a {
    color: aquamarine;
    text-decoration: none;
    margin: 0 2rem;
}
</style>