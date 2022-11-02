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
                subheading: 'Lorem ipsum dolor sit amet consectetur.',
                timeLineBePart: 'Be Part',
                timeLineOfOur: 'Of Our',
                timeLineStory: 'Story!',
                timelines: [
                    {
                        timeLineInverted: '',
                        timeLineImg: require("../assets/img/about/1.jpg"),
                        timeLineHeading: '2009-2011',
                        timeLineSubheading: 'Our Humble Beginnings',
                        timeLineBody: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sunt ut voluptatum eius sapiente, totam reiciendis temporibus qui quibusdam, recusandae sit vero unde, sed, incidunt et ea quo dolore laudantium consectetur!',
                    },
                    {
                        timeLineInverted: 'timeline-inverted',
                        timeLineImg: require("../assets/img/about/2.jpg"),
                        timeLineHeading: 'March 2011',
                        timeLineSubheading: 'An Agency is Born',
                        timeLineBody: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sunt ut voluptatum eius sapiente, totam reiciendis temporibus qui quibusdam, recusandae sit vero unde, sed, incidunt et ea quo dolore laudantium consectetur!',
                    },
                    {
                        timeLineInverted: '',
                        timeLineImg: require("../assets/img/about/3.jpg"),
                        timeLineHeading: 'December 2015',
                        timeLineSubheading: 'Transition to Full Service',
                        timeLineBody: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sunt ut voluptatum eius sapiente, totam reiciendis temporibus qui quibusdam, recusandae sit vero unde, sed, incidunt et ea quo dolore laudantium consectetur!',
                    },
                    {
                        timeLineInverted: 'timeline-inverted',
                        timeLineImg: require("../assets/img/about/4.jpg"),
                        timeLineHeading: 'July 2020',
                        timeLineSubheading: 'Phase Two Expansion',
                        timeLineBody: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sunt ut voluptatum eius sapiente, totam reiciendis temporibus qui quibusdam, recusandae sit vero unde, sed, incidunt et ea quo dolore laudantium consectetur!',
                    }
                ]
            }
        }
    }
</script>

<style>

</style>