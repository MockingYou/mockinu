<template>
  <router-view></router-view>
  <div>
    <base-button class="btn" link to="/" >
      <v-icon aria-label="My Account" role="img" aria-hidden="false">
        mdi-home
      </v-icon>
    </base-button>
    <base-button class="btn" link to="/about" >
      <v-icon aria-label="My Account" role="img" aria-hidden="false">
        mdi-account
      </v-icon>
    </base-button>
    <base-button class="btn" link to="/projects" >
      <v-icon aria-label="My Account" role="img" aria-hidden="false">
        mdi-briefcase
      </v-icon>
    </base-button>
    <base-button class="btn" link to="/contact" >
      <v-icon aria-label="My Account" role="img" aria-hidden="false">
        mdi-email-open
      </v-icon>
    </base-button>
  </div>

</template>

<script>
import HomePage from './pages/HomePage.vue';
import BaseButton from './components/ui/BaseButton.vue';

import { mdiHome, mdiAccount, mdiBriefcase,mdiEmailOpen } from "@mdi/js";

export default {
  data: () => ({
    icons: {
      mdiHome,
      mdiAccount,
      mdiBriefcase ,
      mdiEmailOpen
    }
  }),
  components: {
    HomePage,
    BaseButton
  }
}
</script>

<style scoped>
div {
  position: relative;
  float: right;
  width: 0;
}

</style>
