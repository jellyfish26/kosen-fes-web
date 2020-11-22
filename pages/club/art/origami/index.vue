<template>
  <v-app class="club-page">
    <v-container>
      <v-row no-gutters>
        <v-col class="py-12" cols="12">
          <h1 align="center"> 美術部 </h1>
        </v-col>
      </v-row>
    </v-container>
    <v-container fluid style="width: 85%">
      <v-row no-gutters>
        <v-col class="py-12" cols="12">
          <p class="subtitle" align="left"> 自分で創作した折り紙作品を集めた作品集を作りました！ </p>
          <p class="subtitle" align="left"> 
            付録として展開図や折り方動画付き！
          </p>
          <p class="subtitle" align="left"> 
            興味のある方は是非見てください！
          </p>
        </v-col>
        <v-col cols="12">
          <v-layout align-center>
            <v-icon size="35">mdi-menu-right</v-icon>
            <nuxt-link class="mx-3 title" to="/club/art/origami/way"> 折り方動画 </nuxt-link>
          </v-layout>  
        </v-col>
        <v-col cols="12">
          <v-layout align-center>
            <v-icon size="35">mdi-menu-right</v-icon>
            <a class="mx-3 title" href="https://cdn.nitncfes.net/art/origami/collection.pdf" target=”_blank”> 折り紙作品集 </a>
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