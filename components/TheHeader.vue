<template>
    <b-navbar toggleable="lg" type="dark" variant="dark">
        <b-navbar-brand href="#">
            <img id="navbar-logo" src="~/assets/img/logo-cropped.svg" alt="Logo">
        </b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
            <b-navbar-nav class="ml-auto">
                <b-nav-item to="/">Home</b-nav-item>
                <b-nav-item to="/application">Application</b-nav-item>
            </b-navbar-nav>
        </b-collapse>
    </b-navbar>
</template>

<script>
export default {
    title: "TheHeader"
};
</script>

<style lang="scss">
@import "~assets/scss/_colors.scss";

.navbar {
    font-family: "Fjalla One" !important;
    font-weight: normal;
    text-transform: uppercase;
    font-size: 1.2em;
    padding-left: 20px;
    padding-right: 20px;
    border-bottom: 1px solid map-get($map: $theme-colors, $key: "secondary") !important;
}
#navbar-logo {
    height: 6vh;
}
</style>
