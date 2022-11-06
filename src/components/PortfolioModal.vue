<template>
    <div>
        <div class="portfolio-modal modal fade" id="portfolioModal1" tabindex="-1" role="dialog" aria-hidden="true">
            <div class="modal-dialog">
                <div class="modal-content">
                    <div class="close-modal" data-bs-dismiss="modal"><img v-bind:src="modalDismiss" alt="Close modal" /></div>
                    <div class="container">
                        <div class="row justify-content-center">
                            <div class="col-lg-8">
                                <div class="modal-body">
                                    <!-- Project details-->
                                    <h2 class="text-uppercase">{{ portfolioTitle }}</h2>
                                    <p class="item-intro text-muted">{{ portfolioSubTitle }}</p>
                                    <img class="img-fluid d-block mx-auto"  v-bind:src="portfolioImg" alt="..." />
                                    <p>{{ portfolioBody }}</p>
                                    <ul class="list-inline">
                                        <li>
                                            <strong>Client:</strong>
                                            {{ portfolioClient }}
                                        </li>
                                        <li>
                                            <strong>Category:</strong>
                                            {{ portfolioCategory }}
                                        </li>
                                    </ul>
                                    <button class="btn btn-primary btn-xl text-uppercase" data-bs-dismiss="modal" type="button">
                                        <i class="fas fa-xmark me-1"></i>
                                        {{ closeModalLabel }}
                                    </button>
                                </div>
                            </div>
                        </div>
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
                closeModalLabel: 'Close Project',
                modalDismiss: require("../assets/img/close-icon.svg"),
                portfolioImg: require("../assets/img/portfolio/1.jpg"),
                portfolioClient: 'Threads',
                portfolioCategory: 'Illustration',
                portfolioTitle: 'Project Name',
                portfolioSubTitle: 'Lorem ipsum dolor sit amet consectetur.',
                portfolioBody: 'Use this area to describe your project. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Est blanditiis dolorem culpa incidunt minus dignissimos deserunt repellat aperiam quasi sunt officia expedita beatae cupiditate, maiores repudiandae, nostrum, reiciendis facere nemo!',
            }
        }
    }
</script>

<style>
    
</style>