<template>
    <div>
        <section class="page-section" id="about">
            <div class="container">
                <div class="text-center">
                    <h2 class="section-heading text-uppercase">{{ heading }}</h2>
                    <h3 class="section-subheading text-muted">{{ subheading }}</h3>
                </div>
                <ul class="timeline">
                    <li v-for="timeline in timelines" v-bind:key="timeline.id" v-bind:class="timeline.timeLineInverted">
                        <div class="timeline-image">
                            <img class="rounded-circle img-fluid" v-bind:src="timeline.timeLineImg" alt="..." />
                        </div>
                        <div class="timeline-panel">
                            <div class="timeline-heading">
                                <h4>{{ timeline.timeLineHeading }}</h4>
                                <h4 class="subheading"><h4>{{ timeline.timeLineSubheading }}</h4></h4>
                            </div>
                            <div class="timeline-body"><p class="text-muted">{{ timeline.timeLineBody }}</p></div>
                        </div>
                    </li>
                    <li class="timeline-inverted">
                        <div class="timeline-image">
                            <h4>
                                {{ timeLineBePart }}
                                <br />
                                {{ timeLineOfOur }}
                                <br />
                                {{ timeLineStory }}
                            </h4>
                        </div>
                    </li>
                </ul>
            </div>
        </section>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                heading: 'About',
                subheading: 'We have a clear vision, mission and our own value.',
                timeLineBePart: 'Be Part',
                timeLineOfOur: 'Of Our',
                timeLineStory: 'Story!',
                timelines: [
                    {
                        timeLineInverted: '',
                        timeLineImg: require("../assets/img/about/front-side.png"),
                        timeLineHeading: '',
                        timeLineSubheading: 'Z1 Flexible Solution',
                        timeLineBody: 'is an outstanding IT solution company established with perfectness in mind during the year 2015 and malignly focusing on many areas such as: Property Installment and Clients management system, Project Management, Financial software such as Loan Management System (LMS) product etc….',
                    },
                    {
                        timeLineInverted: 'timeline-inverted',
                        timeLineImg: require("../assets/img/about/back-side.png"),
                        timeLineHeading: '',
                        timeLineSubheading: 'Our Vision',
                        timeLineBody: 'We aim to successfully deliver all our IT projects on time with highly innovative, reliable and maintainable solutions to our clients. we commit to construct long-term relationships with our customers with the purpose of growing together.',
                    },
                    {
                        timeLineInverted: '',
                        timeLineImg: require("../assets/img/about/left-side.png"),
                        timeLineHeading: '',
                        timeLineSubheading: 'Our Mission',
                        timeLineBody: 'With our unique core mission, we target to produce top-class software and provide IT solutions service to every business. In addition, we full-fill the requirements of IT related consulting using cutting-edge technologies with robust development tools and client-oriented perspective.',
                    },
                    {
                        timeLineInverted: 'timeline-inverted',
                        timeLineImg: require("../assets/img/about/right-side.png"),
                        timeLineHeading: '',
                        timeLineSubheading: 'Our Commitment',
                        timeLineBody: 'In term of Talent acquisition, we employ high-class professionals with multiple years of experience in IT in complex projects development and challenging IT solutions. We invest heavily on unique solutions for various businesses within the agreed budget and a timeline. Software products and solutions developed by our technical engineers, are acceptable and follow the standards locally and internationally.',
                    }
                ]
            }
        }
    }
</script>

<style>

</style>