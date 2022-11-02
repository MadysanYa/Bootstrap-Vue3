<template>
    <div>
        <section class="page-section bg-light" id="portfolio">
            <div class="container">
                <div class="text-center">
                    <h2 class="section-heading text-uppercase">{{ heading }}</h2>
                    <h3 class="section-subheading text-muted">{{ subheading }}</h3>
                </div>
                <div class="row">
                    <div class="col-lg-4 col-sm-6 mb-4" v-for="portfolio in portfolios" v-bind:key="portfolio.id">
                        <div class="portfolio-item">
                            <a class="portfolio-link" data-bs-toggle="modal" v-bind:href="portfolio.portfolioLink">
                                <div class="portfolio-hover">
                                    <div class="portfolio-hover-content"><i class="fas fa-plus fa-3x"></i></div>
                                </div>
                                <img class="img-fluid" v-bind:src="portfolio.portfolioImg" alt="..." />
                            </a>
                            <div class="portfolio-caption">
                                <div class="portfolio-caption-heading">{{ portfolio.heading }}</div>
                                <div class="portfolio-caption-subheading text-muted">{{ portfolio.subheading }}</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                heading: 'Portfolio',
                subheading: 'Lorem ipsum dolor sit amet consectetur.',
                portfolios: [
                    {
                        portfolioImg: require("../assets/img/portfolio/1.jpg"),
                        portfolioLink: '#portfolioModal1',
                        heading: 'Threads',
                        subheading: 'Illustration',
                    },
                    {
                        portfolioImg: require("../assets/img/portfolio/2.jpg"),
                        portfolioLink: '#portfolioModal2',
                        heading: 'Explore',
                        subheading: 'Graphic Design',
                    },
                    {
                        portfolioImg: require("../assets/img/portfolio/3.jpg"),
                        portfolioLink: '#portfolioModal3',
                        heading: 'Finish',
                        subheading: 'Identity',
                    },
                    {
                        portfolioImg: require("../assets/img/portfolio/4.jpg"),
                        portfolioLink: '#portfolioModal4',
                        heading: 'Lines',
                        subheading: 'Branding',
                    },
                    {
                        portfolioImg: require("../assets/img/portfolio/5.jpg"),
                        portfolioLink: '#portfolioModal5',
                        heading: 'Southwest',
                        subheading: 'Website Design',
                    },
                    {
                        portfolioImg: require("../assets/img/portfolio/6.jpg"),
                        portfolioLink: '#portfolioModal6',
                        heading: 'Window',
                        subheading: 'Photography',
                    }
                ]
            }
        }
    }
</script>

<style>

</style>