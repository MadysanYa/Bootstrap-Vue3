<template>
    <div>
        <header class="masthead">
            <div class="container">
                <div class="masthead-subheading">{{ subHeading }}</div>
                <div class="masthead-heading text-uppercase">{{ heading }}</div>
                <a class="btn btn-primary btn-xl text-uppercase" v-bind:href="tellMoreLink">{{ tellMore }}</a>
            </div>
        </header>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                subHeading: "Welcome To Our Studio!",
                heading: "It's Nice To Meet You",
                tellMore: "Tell Me More",
                tellMoreLink: "#services",
            }
        }
    }
</script>

<style>

</style>