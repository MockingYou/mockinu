<template>
    <section class="section sec3 active" id="portfolio">
        <div class="main-title">
            <h2>My <span>Projects</span></h2>
        </div>
        <p class="port-text">
            Here are some of my projects that I've done in various programming languages.
        </p>
        <div class="portfolios" v-for="project in projects">
            <div class="portfolio-item">
                <Project :image="project.image" :title="project.title" :description="project.description" />
                <ProjectButton :link="project.link" :icon="project.icon" />
            </div>
        </div>
    </section>
</template>

<script>
import Project from './Project.vue'
import ProjectButton from './ProjectButton.vue'

export default {
    components: {
        Project,
        ProjectButton
    },
     data() {
        return {
            projects: [
                {
                    image: 'topdownshooter.png',
                    title: 'Top down Shooter',
                    description: 'A top down survival game with endless waves of enemies, health pick-ups, enemy death tracker, made using Unreal Engine 4.',
                    link: 'https://drive.google.com/drive/folders/1K4R17y3RalNpESwAOOeHG9F_gO-5KYao?usp=sharing',
                    icon: 'mdi-google-drive',
                },
                {
                    image: 'quiz.png',
                    title: 'Simple Quiz',
                    description: 'A quiz with 5 general knowledge questions, that are provided by an API that is available on opentdb.com.',
                    link: 'https://drive.google.com/drive/folders/1K4R17y3RalNpESwAOOeHG9F_gO-5KYao?usp=sharing',
                    icon: 'mdi-github',
                },
                {
                    image: 'chromeextension.png',
                    title: 'Chrome Extension',
                    description: 'An extension for Chrome that helps you save links and tabs to the local storage.',
                    link: 'https://drive.google.com/drive/folders/1K4R17y3RalNpESwAOOeHG9F_gO-5KYao?usp=sharing',
                    icon: 'mdi-github',
                },
                {
                    image: 'pomodoro.png',
                    title: 'Pomodoro Clock',
                    description: 'A timer that breaks work into intervals separated by short breaks that can be changed by the user.',
                    link: 'https://drive.google.com/drive/folders/1K4R17y3RalNpESwAOOeHG9F_gO-5KYao?usp=sharing',
                    icon: 'mdi-codepen',
                },
            ]
        };
    },
}
</script>