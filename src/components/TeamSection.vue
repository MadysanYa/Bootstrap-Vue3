<template>
    <div>
        <section class="page-section bg-light" id="team">
            <div class="container">
                <div class="text-center">
                    <h2 class="section-heading text-uppercase">{{ heading }}</h2>
                    <h3 class="section-subheading text-muted">{{ subheading }}</h3>
                </div>
                <div class="row">
                    <div class="col-lg-4" v-for="teamMember in teamMembers" v-bind:key="teamMember.id">
                        <div class="team-member">
                            <img class="mx-auto w-auto" v-bind:src="teamMember.teamImage" alt="..." />
                            <h4>{{ teamMember.heading }}</h4>
                            <p class="text-muted">{{ teamMember.subheading }}</p>
                            <!-- <a class="btn btn-dark btn-social mx-2" href="#!" aria-label="Parveen Anand Twitter Profile"><i class="fab fa-twitter"></i></a>
                            <a class="btn btn-dark btn-social mx-2" href="#!" aria-label="Parveen Anand Facebook Profile"><i class="fab fa-facebook-f"></i></a>
                            <a class="btn btn-dark btn-social mx-2" href="#!" aria-label="Parveen Anand LinkedIn Profile"><i class="fab fa-linkedin-in"></i></a> -->
                        </div>
                    </div>
                </div>
                <!-- <div class="row">
                    <div class="col-lg-8 mx-auto text-center">
                        <p class="large text-muted">{{ content }}</p>
                    </div>
                </div> -->
            </div>
        </section>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                heading: 'Our Amazing Products',
                subheading: 'Quality Features',
                content: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aut eaque, laboriosam veritatis, quos non quis ad perspiciatis, totam corporis ea, alias ut unde.',
                teamMembers: [
                    {
                        heading: 'Property Trading',
                        subheading:'Z1 Flexible Solution has challenged the best way of doing things in property investment. We mainly target to transform the property trading industry, provide comfortable way for all traders and increase efficiency with multiple specialized technologies.',
                        teamImage: require("../assets/img/team/vtrust.png"),
                    },
                    {
                        heading: 'Project Managemtn',
                        subheading: "We provide custom software product to align with your company's internal workflow and Standard Operation Procedure. Following international standard from the beginning of software development life cycle: gathering requirements, analysis till maintenance phase.",
                        teamImage: require("../assets/img/team/cic-app.png"),
                    },
                    {
                        heading: 'Loan Management Software',
                        subheading:'Managing loan lifecycle & secured lending online/mobile app, with user friendly dashboards, Manage borrowers, loans, repayments, and reports. Software developed for cash lending industry.',
                        teamImage: require("../assets/img/team/rent-kh.png"),
                    }
                ]
            }
        }
    }
</script>

<style>

</style>