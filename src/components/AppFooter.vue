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
        <div class="container-fluid w-100 bgblue">
            <div class="col-12">
                <div class="d-flex row g-0 cicle1">
                    <div class="link-item" v-for="link in links" :key="link.title">
                        <img :src="link.image[0]" :alt="link.title" />
                        <p>{{ link.title }}</p>
                    </div>
                </div>
            </div>
        </div>

        <div class="container-fluid w-100 bgimage p-5">
            <div class="d-flex row g-0">
                <div class="col-2">
                    
                    <ul>
                        <li><h3 class="text-white">DC COMICS</h3></li>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>

                    

                    <ul>
                        <li><h3 class="text-white">SHOP</h3></li>
                        <li>Shop DC</li>
                        <li>Shop Collectibles</li>
                    </ul>

                </div>

                <div class="col-2 ">
                    

                    <ul>
                        <li><h3 class="text-white">DC</h3></li>
                        <li>Terms of Use</li>
                        <li>Privacy policy (New)</li>
                        <li>Ad Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscription</li>
                        <li>Talent Workshops</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                </div>

                <div class="col-2">
                    <ul>
                        <li><h3 class="text-white">SITES</h3></li>
                        <li>DC</li>
                        <li>Mad Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>

                    </ul>
                </div>
            </div>


        </div>
    </footer>
</template>

<style scoped>
footer {
    color: white;
}

footer>.bgblue {
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

/* 2° CONTENITORE */

.bgimage{
    background-image: url(/public/img/footer-bg.jpg);
    height: 40vh;

}

li{
    color: grey;
    margin-left: 35px;
    list-style-type: none;
}

ul{
    padding: 0;
    
}

.d-flex{
    justify-content: center;
    align-items: start;
    padding: 15px;
}
</style>