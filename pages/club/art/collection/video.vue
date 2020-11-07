<template>
  <v-app class="club-page">
    <v-container>
      <v-row no-gutters>
        <v-col class="py-12" cols="12">
          <h1 align="center"> 美術部 </h1>
        </v-col>
        <v-col class="py-12" cols="12">
          <h2 align="center"> 自由作品動画 </h2>
        </v-col>
      </v-row>
    </v-container>
     <v-container style="width: 85%">
      <HLSVideo
        src="https://cdn.nitncfes.net/art/main/video.m3u8"
      />
      <v-row no-gutters>
        <v-col cols="12">
           <p class="py-3 title font-weight-bold" align="center"> 参考文献 </p>
        </v-col>
        <v-col class="py-3" cols="12">
          <p class="subtitle" align="left"> 
            風車の絵:『暮らしてみたい 世界のかわいい街』発行:エムディエヌコーポレーション 発行年:2019 pp.74-75 
          </p>
          <p class="subtitle" align="left"> 
            海の絵:上に同じ、p.67
          </p>
          <p class="subtitle" align="left"> 
            赤毛のアンの家:『まるで童話のような 世界のかわいい村と美しい街』発行:パイ インターナショナル 発行年:2016 p.21
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