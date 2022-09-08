<template>
    <div v-for="project in projects" class="portfolio-item">
        <div class="image">
            <img v-bind:src="'../img/' + project.image" alt="" />
        </div>
        <div class="hover-items">
            <h3>{{ project.title}}</h3>
            <p class="project-desc">{{ project.description }}</p>
            <ProjectButton />
        </div>
    </div>
</template>

<script>
import ProjectButton from './ProjectButton.vue'
export default {
    components: {
        ProjectButton
    },
    data() {
        return {
            projects: [
                {
                    image: 'topdownshooter.png',
                    title: 'Top down Shooter',
                    description: '>A top down survival game with endless waves of enemies, health pick-ups, enemy death tracker, made using Unreal Engine 4.'
                },
                {
                    image: 'quiz.png',
                    title: 'Simple Quiz',
                    description: 'A quiz with 5 general knowledge questions, that are provided by an API that is available on opentdb.com.'
                },
                {
                    image: 'chromeextension.png',
                    title: 'Chrome Extension',
                    description: 'An extension for Chrome that helps you save links and tabs to the local storage.'
                },
                {
                    image: 'pomodoro.png',
                    title: 'Pomodoro Clock',
                    description: 'A timer that breaks work into intervals separated by short breaks that can be changed by the user.'
                },

            ],
        };
    },
}
</script>