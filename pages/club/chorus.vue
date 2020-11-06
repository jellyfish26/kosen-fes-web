<template>
  <v-app class="club-page">
    <v-container>
      <v-row no-gutters>
        <v-col class="py-12" cols="12">
          <h1 align="center"> 合唱同好会 </h1>
        </v-col>
      </v-row>
    </v-container>
    <v-container fluid style="width: 85%">
      <v-row no-gutters>
        <v-col class="pa-2" cols="12">
          <v-layout justify-center>
            <v-img
              max-width="700px"
              src="https://cdn.nitncfes.net/chorus/chorus.jpg"
            > </v-img>
          </v-layout>
        </v-col>
        <v-col class="py-12" cols="12">
          <v-col class="pa-2" cols="12">
          <p class="subtitle" align="left"> 合唱同好会は、毎週木曜の15:30〜16:30まで、凌雲館2F(購買の上です)の南多目的室で活動しています！ </p>
          <p class="subtitle" align="left"> 
            メインイベントは高専祭のステージと卒業式・入学式で、去年の高戦災では映画「天使にラブソングを」で知られるHail Holy Queenや、
            松田聖子さんでおなじみの瑠璃色の地球を歌いました。
          </p>
          <p class="subtitle" align="left"> 
            週1時間だけの活動なので他の部活と兼部しやすく、予定の都合もつきやすいのが魅力です。
          </p>
          <p class="subtitle" align="left"> 
            日々のちょっとした息抜きに、一緒に歌いませんか？新入部員大募集中です！どなたでも気軽に歌いに来てください。
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