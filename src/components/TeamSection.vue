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
                            <img class="mx-auto rounded-circle" v-bind:src="teamMember.teamImage" alt="..." />
                            <h4>{{ teamMember.heading }}</h4>
                            <p class="text-muted">{{ teamMember.subheading }}</p>
                            <a class="btn btn-dark btn-social mx-2" href="#!" aria-label="Parveen Anand Twitter Profile"><i class="fab fa-twitter"></i></a>
                            <a class="btn btn-dark btn-social mx-2" href="#!" aria-label="Parveen Anand Facebook Profile"><i class="fab fa-facebook-f"></i></a>
                            <a class="btn btn-dark btn-social mx-2" href="#!" aria-label="Parveen Anand LinkedIn Profile"><i class="fab fa-linkedin-in"></i></a>
                        </div>
                    </div>
                </div>
                <div class="row">
                    <div class="col-lg-8 mx-auto text-center">
                        <p class="large text-muted">{{ content }}</p>
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
                heading: 'Our Amazing Team',
                subheading: 'Lorem ipsum dolor sit amet consectetur.',
                content: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aut eaque, laboriosam veritatis, quos non quis ad perspiciatis, totam corporis ea, alias ut unde.',
                teamMembers: [
                    {
                        heading: 'Parveen Anand',
                        subheading:'Lead Marketer',
                        teamImage: require("../assets/img/team/1.jpg"),
                    },
                    {
                        heading: 'Diana Petersen',
                        subheading:'Lead Designer',
                        teamImage: require("../assets/img/team/2.jpg"),
                    },
                    {
                        heading: 'Larry Parker',
                        subheading:'Lead Developer',
                        teamImage: require("../assets/img/team/3.jpg"),
                    }
                ]
            }
        }
    }
</script>

<style>

</style>