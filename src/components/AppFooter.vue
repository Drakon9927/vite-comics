<script>
export default {
    data() {
        return {
            links: ["Privacy", "Termini"]
        }
    }
}
</script>

<template>
    <footer>
        Realizzato con: 
        <img class="logo" src="/vite.svg" />
        +
        <img class="logo" src="../assets/vue.svg" />
        <div>
            <a v-for="link in links" :href="'#' + link.toLowerCase()">{{ link }}</a>
        </div>
    </footer>
</template>

<style scoped>
footer {
    background-color: #444;
    padding: 1rem;
    text-align: center;
    color: white;
}

img.logo {
    height: 1rem;
    transition: all 300ms;
}
img.logo:hover {
    transform: scale(1.75);
}

a {
    color: aquamarine;
    text-decoration: none;
    margin: 0 2rem;
}
</style>