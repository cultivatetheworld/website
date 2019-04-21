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
                    class="display-4"
                >Decentralizing weather stations to maximize agricultural production.</h1>
                <div class="text-center py-4">
                    <a v-scroll-to="'#index-mission'">
                        <i class="fas fa-arrow-down"></i>
                    </a>
                </div>
            </div>
        </b-container>
        <b-container id="index-mission" class="text-center m-block">
            <h1>Mission</h1>
            <p>
                Our mission is to collect and analyze weather data by leveraging cloud-based machine learning techniques to provide valuable
                insights into weather patterns and reduce crop failure.
            </p>
        </b-container>
        <b-container class="text-center m-block">
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

<style lang="scss">
@import "~assets/scss/_colors.scss";

#index-hero {
    background-image: linear-gradient(
            rgba(
                darken(map-get($map: $theme-colors, $key: "success"), 40%),
                0.5
            ),
            rgba(
                darken(map-get($map: $theme-colors, $key: "success"), 50%),
                0.5
            )
        ),
        url("~assets/img/index-hero.jpg");

    min-height: 90vh;
    background-size: cover;
    background-position: center center;
    background-repeat: no-repeat;
    background-attachment: fixed;
    padding: 20px;
    padding-bottom: 80px;

    i {
        font-size: 3em;
        opacity: 0.8;
        padding-top: 50px;
        animation: blink 2s linear infinite;
        cursor: pointer;
    }
}
#index-hero-text {
    padding-top: 30vh;
    padding-left: 10vw;
    padding-right: 10vw;
    font-weight: bold;
    line-height: 80px;
}
</style>
