<template>
  <router-view></router-view>
  <div class="controls">
    <base-button class="control  control-1" link to="/" >
      <v-icon aria-label="My Account" role="img" aria-hidden="false">
        mdi-home
      </v-icon>
    </base-button>
    <base-button class="control  control-1" link to="/about" >
      <v-icon aria-label="My Account" role="img" aria-hidden="false">
        mdi-account
      </v-icon>
    </base-button>
    <base-button class="control  control-1" link to="/projects" >
      <v-icon aria-label="My Account" role="img" aria-hidden="false">
        mdi-briefcase
      </v-icon>
    </base-button>
    <base-button class="control  control-1" link to="/contact" >
      <v-icon aria-label="My Account" role="img" aria-hidden="false">
        mdi-email-open
      </v-icon>
    </base-button>
  </div>
  <div class="theme-btn">
    <theme-button @click="updateTheme"></theme-button>  
  </div>
</template>

<script>
import HomePage from './pages/HomePage.vue';
import BaseButton from './components/ui/BaseButton.vue';
import ThemeButton from './components/ui/ThemeButton.vue';
import { RouterLink, RouterView } from 'vue-router'
import ProjectPage from './pages/ProjectPage.vue'

import { mdiHome, mdiAccount, mdiBriefcase,mdiEmailOpen } from "@mdi/js";

export default {
  data: () => ({
    icons: {
      mdiHome,
      mdiAccount,
      mdiBriefcase ,
      mdiEmailOpen
    },
    isActive: false,
    currentTheme : ''
  }),
  components: {
    HomePage,
    BaseButton,
    ProjectPage,
    ThemeButton
  },
  methods: {
    updateTheme() {
        let element = document.body;
        element.classList.toggle('light-mode')
    }
  }
}
</script>

<!-- <style>
body {
  background-color: #191d2b;
  font-family: 'Poppins', sans-serif;
  font-size: 1.1rem;
  color: #FFFFFF;
  -webkit-transition: all .4s ease-in-out;
  transition: all .4s ease-in-out;
}

div {
  position: relative;
  float: right;
  width: 0;
}

</style> -->
