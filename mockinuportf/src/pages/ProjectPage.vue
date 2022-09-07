<template>
    <section class="section sec3" id="portfolio">
        <div class="main-title">
            <h2>My <span>Projects</span></h2>
        </div>
        <p class="port-text">
            Here is some of my work that I've done in various programming languages.
        </p>
        <div class="portfolios">
            <Project />
        </div>
    </section>
</template>

<script>
import Project from './Project.vue'

export default {
    components: {
        Project
    }
}
</script>