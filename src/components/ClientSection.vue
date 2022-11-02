<template>
    <div>
        <div class="py-5">
            <div class="container">
                <div class="row align-items-center">
                    <div class="col-md-3 col-sm-6 my-3" v-for="clientImg in clientImgs" v-bind:key="clientImg.id">
                        <a href="#!"><img class="img-fluid img-brand d-block mx-auto" v-bind:src="clientImg.imgBrand" alt="..." aria-label="Microsoft Logo" /></a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                clientImgs: [
                    {
                        imgBrand: require("../assets/img/logos/microsoft.svg"),
                    },
                    {
                        imgBrand: require("../assets/img/logos/google.svg"),
                    },
                    {
                        imgBrand: require("../assets/img/logos/facebook.svg"),
                    },
                    {
                        imgBrand: require("../assets/img/logos/ibm.svg"),
                    },
                ]
            }
        }
    }
</script>

<style>

</style>