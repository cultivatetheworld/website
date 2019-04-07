<template>
    <div>
        <link
            rel="stylesheet"
            href="https://use.fontawesome.com/releases/v5.8.1/css/all.css"
            integrity="sha384-50oBUHEmvpQ+1lW4y57PTFmhCaXp0ML5d60M1M7uH2+nqUivzIebhndOJK28anvf"
            crossorigin="anonymous"
        >
        <TheHeader/>
        <b-container id="index-hero" class="text-center" fluid>
            <div>
                <h1
                    id="index-hero-text"
                    class="font-italic"
                >Decentralizing weather stations to maximize agricultural production.</h1>
                <div class="text-center py-4">
                    <a v-scroll-to="'#index-mission'">
                        <i class="fas fa-arrow-down"></i>
                    </a>
                </div>
            </div>
        </b-container>
        <b-container id="index-mission" class="text-center my-4">
            <h1>Mission</h1>
            <p>
                Our mission is to collect and analyze weather data by leveraging cloud-based machine learning techniques to provide valuable
                insights into weather patterns and reduce crop failure.
            </p>
        </b-container>
        <b-container class="text-center my-4">
            <h1>Inspiration</h1>
            <p>
                Food production is what drives the development of the world. In many developing countries, the crop yield isn't sufficient to satisfy the needs of an ever-growing population.
                We decided to pursue the difficult task of solving this issue, and created Cultivate the World.
            </p>
        </b-container>
    </div>
</template>

<script>
import TheHeader from "~/components/TheHeader.vue";

export default {
    components: {
        TheHeader
    }
};
</script>

<style>
html,
body {
    font-family: "Imprima", sans-serif;
    background-color: #435058;
    color: #f1f2ee;
}
#index-hero {
    padding: 0px;
    background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
        url("~assets/img/index-hero.jpg");
    height: 90vh;
    background-size: cover;
    background-position: center center;
    background-repeat: no-repeat;
    background-attachment: fixed;
}
#index-hero i {
    font-size: 5em;
    opacity: 0.5;
    padding-top: 50px;
}
#index-hero-text {
    padding-top: 30vh;
    padding-left: 10vw;
    padding-right: 10vw;
}
</style>
