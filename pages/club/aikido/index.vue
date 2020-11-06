<template>
  <v-app class="club-page">
    <v-container>
      <v-row no-gutters>
        <v-col class="py-12" cols="12">
          <h1 align="center"> 合気道部 </h1>
        </v-col>
      </v-row>
    </v-container>
    <v-container style="width: 85%">
      <v-row no-gutters>
        <v-col cols="12">
          <v-layout align-center>
            <v-icon size="35">mdi-menu-right</v-icon>
            <nuxt-link class="mx-3 title" to="/club/aikido/promotion"> プロモーションビデオ </nuxt-link>
          </v-layout>  
        </v-col>
        <v-col cols="12">
          <v-layout align-center>
            <v-icon size="35">mdi-menu-right</v-icon>
            <a class="mx-3 title" href="https://cdn.nitncfes.net/aikido/poster.pdf" target=”_blank”> ポスター </a>
          </v-layout>  
        </v-col>
      </v-row>
    </v-container>
  </v-app>
</template>

<style scoped>
.club-page {
  background: url('~assets/struckaxiom.png') fixed repeat round;
}
</style>

<script>
import HLSVideo from '@/components/HLSVideo'

export default {
  components: {
    HLSVideo
  },
  data() {
    return {
    }
  }
}
</script>