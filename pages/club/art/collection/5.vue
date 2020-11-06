<template>
  <v-app class="club-page">
    <v-container>
      <v-row no-gutters>
        <v-col class="py-12" cols="12">
          <h1 align="center"> 美術部 </h1>
        </v-col>
        <v-col class="py-12" cols="12">
          <h2 align="center"> カエル </h2>
        </v-col>
      </v-row>
    </v-container>
    <v-container fluid style="width: 85%">
      <v-row no-gutters>
        <v-col class="py-3" cols="12" >
          <v-layout justify-center>
            <v-img
              max-width="350px"
              src="https://cdn.nitncfes.net/art/collection/5/first.jpg"
            > </v-img>
          </v-layout>
        </v-col>
        <v-col class="py-3" cols="12" >
          <v-layout justify-center>
            <v-img
              max-width="350px"
              src="https://cdn.nitncfes.net/art/collection/5/second.jpg"
            > </v-img>
          </v-layout>
        </v-col>
        <v-col cols="12">
           <p class="py-3 title font-weight-bold" align="center"> 作品の説明 </p>
        </v-col>
        <v-col class="py-3" cols="12">
          <p class="subtitle" align="left"> 
            折り紙のアマガエルです。 
            神谷哲史さん創作で、折り図を見ながら作りました。 
            紙の裏面で白いお腹を表現しており、「インサイドアウト」と呼ばれる技法です。 
            和紙を使い、柔らかな雰囲気に仕上げました。 
          </p>
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