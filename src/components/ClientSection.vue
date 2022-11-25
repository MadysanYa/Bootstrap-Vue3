<template>
    <div>
        <div class="py-5 bg-light">
            <div class="container">
                <div class="row align-items-center">
                    <div class="col-md-2 col-sm-6 my-3" v-for="clientImg in clientImgs" v-bind:key="clientImg.id">
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
                        imgBrand: require("../assets/img/logos/vtrust.png"),
                    },
                    {
                        imgBrand: require("../assets/img/logos/park-cafe.png"),
                    },
                    {
                        imgBrand: require("../assets/img/logos/rent-kh.png"),
                    },
                    {
                        imgBrand: require("../assets/img/logos/shg.png"),
                    },
                    {
                        imgBrand: require("../assets/img/logos/21.png"),
                    },
                    {
                        imgBrand: require("../assets/img/logos/cic.png"),
                    },
                ]
            }
        }
    }
</script>

<style>

</style>