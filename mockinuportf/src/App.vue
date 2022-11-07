<template>
  <router-view></router-view>
  <div>
    <base-button class="btn" link to="/" >Home</base-button>
    <base-button class="btn" link to="/about" >About</base-button>
    <base-button class="btn" link to="/projects" >Projects</base-button>
    <base-button class="btn" link to="/contact" >Contact</base-button>
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
  float: right;
  width: 0;
}

</style>
