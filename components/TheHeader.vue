<template>
    <b-navbar toggleable="lg" type="dark" variant="info">
        <b-navbar-brand href="#">
            <img id="navbar-logo" src="~/assets/img/logo.png" alt="Logo">
        </b-navbar-brand>
        <b-navbar-brand href="#" class="text-uppercase" id="navbar-header">Cultivate the World</b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
            <b-navbar-nav class="ml-auto">
                <b-nav-item to="/">Home</b-nav-item>
                <b-nav-item to="/about">About</b-nav-item>
                <b-nav-item to="/demo">Demo</b-nav-item>
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
    font-family: "Imprima", sans-serif !important;
}
#navbar-logo {
    max-height: 30px;
}
#navbar-header {
    font-family: "Imprima";
}
</style>
