<template>
  <v-app class="club-page">
    <v-container>
      <v-row no-gutters>
        <v-col class="py-12" cols="12">
          <h1 align="center"> 美術部 </h1>
        </v-col>
        <v-col class="py-12" cols="12">
          <h2 align="center"> イラスト </h2>
        </v-col>
      </v-row>
    </v-container>
    <v-container fluid style="width: 85%">
      <v-row no-gutters>
        <v-col class="py-3" cols="12" >
          <v-layout justify-center>
            <v-img
              src="https://cdn.nitncfes.net/art/collection/7/first.jpeg"
            > </v-img>
          </v-layout>
        </v-col>
        <v-col class="py-3" cols="12" >
          <v-layout justify-center>
            <v-img
              src="https://cdn.nitncfes.net/art/collection/7/second.jpeg"
            > </v-img>
          </v-layout>
        </v-col>
        <v-col class="py-3" cols="12" >
          <v-layout justify-center>
            <v-img
              src="https://cdn.nitncfes.net/art/collection/7/third.jpeg"
            > </v-img>
          </v-layout>
        </v-col>
        <v-col cols="12">
           <p class="py-3 title font-weight-bold" align="center"> 作品の説明 </p>
        </v-col>
        <v-col class="py-3" cols="12">
          <p class="subtitle" align="left"> 
            風車とチューリップの絵:オランダのアムステルダムの郊外にあるチューリップ畑と風車を透明水彩で描きました。空の色が透明水彩の長所を生かしてきれいにできたと思います。 
          </p>
          <p class="subtitle" align="left"> 
            海の絵:クロアチアのドゥブロヴニクから見える風景を透明水彩で描きました。 
          </p>
          <p class="subtitle" align="left"> 
            家の絵:「赤毛のアン」の舞台、カナダのプリンス・エドワード島にある、物語で従姉妹が住んでいたグリーンゲイブルズを透明水彩で書きました。家自体はかなり忠実に再現できたと思います。 
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