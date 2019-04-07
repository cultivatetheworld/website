<template>
    <div>
        <TheHeader/>
        <b-container>
            <div>
                <h1>
                    Welcome,
                    <strong>User</strong>
                </h1>
            </div>
        </b-container>
        <b-container class="my-4">
            <h1>Current Data</h1>
            <b-row>
                <b-col cols="6">Temperature: 40 C</b-col>
                <b-col cols="6">Altitude: 11 m</b-col>
                <b-col cols="6">Pressure: 101 kPa</b-col>
                <b-col cols="6">Humidity: 14%</b-col>
            </b-row>
        </b-container>
        <b-container class="my-4">
            <h1>Future Predictions</h1>
            <p>Implementation coming soon!</p>
        </b-container>
        <b-container class="my-4">
            <blockquote>
                <h4>Contact your local politician in order to make this dream a reality!</h4>
            </blockquote>
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

.container {
    padding-top: 30px;
}
</style>
