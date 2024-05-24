<script>
export default {
    data() {
        return {
            links: ["Characters", "Comics", "Movies", "TV", "Characters", "Games", "Collectibles", "Videos", "Fans", "News", "Shop"],
            logo: ["dc-logo.png"]
        }
    }
}
</script>

<template>
    <header>
        <div class="container-fluid">
            <div class="d-flex row g-0">
                <div class="col-5">
                    <img :src="logo[0]" alt="DC Logo">
                </div>
                <div class="col-7">
                    <ul class="horizontal-links">
                        <li v-for="link in links" :key="link">
                            {{ link }}
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </header>
</template>

<style scoped>
header {
    height: 3rem;
    padding: 1rem;
    max-width: 80%;
    background-color: white;
    margin: 0 auto;
}

.horizontal-links {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex; 
}

.horizontal-links li {
    margin-right: 20px; 
}
</style>