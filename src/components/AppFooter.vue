<script>
export default {
    data() {
        return {
            links: [
        {
            image: ["/public/img/buy-comics-digital-comics.png"],
            title: 'DIGITAL COMICS',
            
        }, {
            image: ["/public/img/buy-comics-merchandise.png"],
            title: 'DC MERCHANDISE',
           
        }, {
            image: ["/public/img/buy-comics-subscriptions.png"],
            title: 'SUBSCRIPTION',
            
        }, {
            image: ["/public/img/buy-comics-shop-locator.png"],
            title: 'COMIC SHOP LOCATOR',
            
        }, {
            image: ["/public/img/buy-dc-power-visa.svg"],
            title: "DC POWER VISA",
            
        }
    ]

            
        }
    }
}
</script>

<template>
    <footer>
        <div class="container-fluid w-100">
            <div class="col-12">
                <div class="d-flex row g-0 cicle1">
                    <div class="link-item" v-for="link in links" :key="link.title">
                        <img :src="link.image[0]" :alt="link.title" />
                        <p>{{ link.title }}</p>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<style scoped>
footer {
    color: white;
}

footer>.container-fluid {
    background-color: #0282F9;
}

.container-fluid>.col-12{
    max-width: 60%;
    margin: 0 auto;
}

.cicle1>.link-item img {
    width: 50px; 
    height: auto; 
}

.d-flex {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
}

.link-item {
    flex: 1 1 20%;
    text-align: center;
    display: flex; 
    align-items: center; 
    justify-content: center; 
}

.link-item p {
    margin-left: 10px; 
}
</style>