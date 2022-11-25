<template>
    <div>
        <section class="page-section" id="services">
            <div class="container">
                <div class="text-center">
                    <h2 class="section-heading text-uppercase">{{ heading }}</h2>
                    <h3 class="section-subheading text-muted">{{ subheading }}</h3>
                </div>
                <div class="row text-center">
                    <div class="col-md-4" v-for="solution in solutions" :key="solution.id">
                        <span class="fa-stack fa-4x">
                            <em class="fas fa-circle fa-stack-2x text-primary"></em>
                            <em class="fas fa-stack-1x fa-inverse" :class="[solution.iconName]"></em>
                        </span>
                        <h4 class="my-3">{{ solution.heading }}</h4>
                        <p class="text-muted">{{ solution.subheading }}</p>
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
                heading: 'Meet Our Solutions',
                subheading: 'Why Customers Love Us',
                solutions: [
                    {
                        heading: 'Ultimate Customization',
                        subheading:"We have great ambitions and dedicate ourselves to gather customer's requirement for features or extension modification of software demanding custom coding or other form of implementation.",
                        iconName: 'fa-shopping-cart',
                    },
                    {
                        heading: 'Scale Up Your Business',
                        subheading: "We offer a complete set of tools and platforms to grow and manage your organization. A range of systems for HR, IT, Finance, Marketing and Sales departments.",
                        iconName: 'fa-laptop fa-stack-1x',
                    },
                    {
                        heading: 'Day to day IT Support',
                        subheading:'Is Your existing IT team unable to Solve IT Issues within business? We can provide certified IT support team to your office and responsible for daily IT support/Helpdesk and training allowing your business to grow even faster.',
                        iconName: 'fa-lock fa-stack-1x',
                    }
                ],
            }
        },
    }
</script>

<style>

</style>