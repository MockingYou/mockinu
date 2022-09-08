<template>
  <router-view></router-view>
  <div>
    <base-button link to="/" >Home</base-button>
    <base-button link to="/about" >About</base-button>
    <base-button link to="/projects" >Projects</base-button>
    <base-button link to="/contact" >Contact</base-button>
  </div>

</template>

<script>
import HomePage from './pages/HomePage.vue';
import BaseButton from './components/ui/BaseButton.vue';


export default {
  components: {
    HomePage,
    BaseButton
  }
}
</script>

<style scoped>
div {
  display: inline-block;
  width: 50%;
}
</style>
