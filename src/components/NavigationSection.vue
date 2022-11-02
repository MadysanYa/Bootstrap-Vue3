<template>
    <div>
        <nav class="navbar navbar-expand-lg navbar-dark fixed-top" id="mainNav">
            <div class="container">
                <a class="navbar-brand" href="#page-top">
                    <img v-bind:src="logo" alt="navbar-logo.svg">
                </a>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarResponsive" aria-controls="navbarResponsive" aria-expanded="false" aria-label="Toggle navigation">
                    {{ label }}<i class="fas fa-bars ms-1"></i>
                </button>
                <div class="collapse navbar-collapse" id="navbarResponsive">
                    <ul class="navbar-nav text-uppercase ms-auto py-4 py-lg-0">
                        <li class="nav-item" v-for="(menu, index) in menus" :key="menu.id">
                            <a class="nav-link" v-bind:href="'#'+index">{{ menu }}</a>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                logo: require("../assets/img/navbar-logo.svg"),
                label: 'Menu',
                menus: {
                    services: 'Services',
                    portfolio: 'Portfolio',
                    about: 'About',
                    team: 'Team',
                    contact: 'Contact',
                }
            }
        }
    }
</script>

<style>

</style>