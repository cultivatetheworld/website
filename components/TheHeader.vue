<template>
    <b-navbar toggleable="lg" type="dark" variant="info">
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

<style>
.navbar {
    background-color: #435058 !important;
    font-family: "Didact Gothic" !important;
    font-weight: bold;
    font-size: 1.2em;
    padding-left: 20px;
    padding-right: 20px;
}
#navbar-logo {
    height: 8vh;
}
</style>
