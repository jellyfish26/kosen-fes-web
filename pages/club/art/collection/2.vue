<template>
  <v-app class="club-page">
    <v-container>
      <v-row no-gutters>
        <v-col class="py-12" cols="12">
          <h1 align="center"> 美術部 </h1>
        </v-col>
        <v-col class="py-12" cols="12">
          <h2 align="center"> Bloom Forever </h2>
        </v-col>
      </v-row>
    </v-container>
    <v-container fluid style="width: 85%">
      <v-row no-gutters>
        <v-col class="py-3" cols="12" >
          <v-layout justify-center>
            <v-img
              src="https://cdn.nitncfes.net/art/collection/2/first.jpg"
            > </v-img>
          </v-layout>
        </v-col>
        <v-col class="py-3" cols="12" >
          <v-layout justify-center>
            <v-img
              src="https://cdn.nitncfes.net/art/collection/2/second.jpg"
            > </v-img>
          </v-layout>
        </v-col>
        <v-col cols="12">
           <p class="py-3 title font-weight-bold" align="center"> 作品の説明 </p>
        </v-col>
        <v-col class="py-3" cols="12">
          <p class="subtitle" align="left"> 
            木に沢山の紙飛行機を咲かせた作品となります。
            作品にこめた思いとしては、
            「一度抱いた夢は叶うまでは夢であり、それが現実になるまでに挫折を経験したり、自身が気づかない間に自然と忘れてしまったり。
            それをぼくたち子どもは夢を手にするまでに当たり前のように、何度も繰り返していくうちに夢の数が多くなっていく。」その様子を表現してみました。 
          </p>
          <p class="subtitle" align="left"> 
            今までは、ケッテンクラートのように紙工作でリアルを追求していたのですが、今回は初めて完全に創作となる作品に挑戦しました。一度は作ってみたかったので高専祭に間に合ってよかったです。 
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