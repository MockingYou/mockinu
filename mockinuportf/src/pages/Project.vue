<template>
    <!-- <div v-for="project in projects" class="portfolio-item"> -->
    <div class="portfolio-item">    
        <div class="image">
            <img v-bind:src="'../img/' + image" alt="" />
        </div>
        <div class="hover-items">
            <div
                v-text="title"
            />
            <div class="project-desc"
                v-text="description"
            />
        </div>
    </div>
</template>

<script>
export default {
    name: 'Project',
    props: {
        image:  String,
        title: String,
        description: String
    },
    // data() {
    //     return {
    //         projects: [
    //             {
    //                 image: 'topdownshooter.png',
    //                 title: 'Top down Shooter',
    //                 description: '>A top down survival game with endless waves of enemies, health pick-ups, enemy death tracker, made using Unreal Engine 4.'
    //             },
    //             {
    //                 image: 'quiz.png',
    //                 title: 'Simple Quiz',
    //                 description: 'A quiz with 5 general knowledge questions, that are provided by an API that is available on opentdb.com.'
    //             },
    //             {
    //                 image: 'chromeextension.png',
    //                 title: 'Chrome Extension',
    //                 description: 'An extension for Chrome that helps you save links and tabs to the local storage.'
    //             },
    //             {
    //                 image: 'pomodoro.png',
    //                 title: 'Pomodoro Clock',
    //                 description: 'A timer that breaks work into intervals separated by short breaks that can be changed by the user.'
    //             },

    //         ],
    //     };
    // },
}
</script>