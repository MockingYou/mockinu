<template>
    <div class="portfolio-item">
        <div class="image">
            <img src="../img/topdownshooter.png" alt="">
        </div>
        <div class="hover-items">
            <h3>Top-down Shooter</h3>
            <p class="project-desc">A top down survival game with endless waves of enemies, health pick-ups, enemy death tracker, made using Unreal Engine 4.</p>
            <ProjectButton />
        </div>
    </div>
</template>

<script>
import ProjectButton from './ProjectButton.vue'
export default {
    components: {
        ProjectButton
    }
}
</script>