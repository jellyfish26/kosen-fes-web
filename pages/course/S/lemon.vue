<template>
  <v-app class="club-page">
    <v-container>
      <v-row no-gutters>
        <v-col class="py-12" cols="12">
          <h1 align="center"> 電子制御工学科 </h1>
        </v-col>
        <v-col class="py-12" cols="12">
          <h2 align="center"> 【光る自動演奏ハンドベル】『米津玄師 - Lemon』を演奏してみた。 </h2>
        </v-col>
      </v-row>
    </v-container>
     <v-container style="width: 85%">
       <v-layout justify-center>
         <YoutubeVideo
          id="RXvnkIhzTCE"
        />
       </v-layout>
    </v-container>
  </v-app>
</template>

<style scoped>
.club-page {
  background: url('~assets/ep_naturalwhite.png') fixed repeat round;
}
</style>

<script>
import YoutubeVideo from '@/components/YoutubeVideo'

export default {
  components: {
    YoutubeVideo
  },
  data() {
    return {
    }
  }
}
</script>