
<template style="background-color: #FCFDC7;">
  <v-app>
    <v-main style="background-color: #FCFDC7;">
      <v-container fill-height>
        <v-row justify="center" align="center">
          <v-col cols="12" sm="8" md="6">
            <LogoComponent class="mt-12"/>
            <ComingSoonComponent class="mt-28"/>
          </v-col>
        </v-row>
      </v-container>
    </v-main>
    <FooterComponent/>
  </v-app>
</template>

<script>
import LogoComponent from "./components/LogoComponent.vue";
import ComingSoonComponent from "./components/ComingSoonComponent.vue";
import FooterComponent from "./components/FooterComponent.vue";
export default {
  name: 'App',
  components: {
    FooterComponent,
    LogoComponent,
    ComingSoonComponent
  }
}
</script>

<style>
@tailwind base;
@tailwind components;
@tailwind utilities;
@import url('https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap');
body {
  font-family: 'Press Start 2P', cursive;
}
</style>
