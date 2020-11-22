<template>
  <v-app class="club-page">
    <v-container>
      <v-row no-gutters>
        <v-col class="py-12" cols="12">
          <h1 align="center"> 情報工学科 </h1>
        </v-col>
      </v-row>
    </v-container>
    <v-container style="width: 85%">
      <v-row no-gutters>
        <v-col cols="12">
          <v-layout align-center>
            <v-icon size="35">mdi-menu-right</v-icon>
            <a class="mx-3 title" href="https://clicker.nitncfes.net" target=”_blank”> しかせんべいくりっかー </a>
          </v-layout>  
        </v-col>
        <v-col cols="12">
          <p class="subtitle" align="left"> 
            しかせんべいくりっかーです。クリックやタップしまくって鹿せんべいを沢山増やそう！
          </p>
          <p class="subtitle" align="left"> 
            そして、溜まった鹿せんべいで施設を購入し、さらに増産しよう！！
          </p>
          <p class="subtitle" align="left"> 
            大量の実績が待っています！みんなで協力して実績を解除していこう！
          </p>
        </v-col>
        <v-col cols="12">
          <v-layout align-center>
            <v-icon size="35">mdi-menu-right</v-icon>
            <a class="mx-3 title" href="https://reversi.nitncfes.net" target=”_blank”> かすたむりばーし </a>
          </v-layout>  
        </v-col>
        <v-col cols="12">
          <p class="subtitle" align="left"> 
            なぞなAIと自分でカスタマイズしたリバーシで対戦できます。負けるほうが難しいかも…？！
          </p>
        </v-col>
        <v-col cols="12">
          <v-layout align-center>
            <v-icon size="35">mdi-menu-right</v-icon>
            <a class="mx-3 title" href="https://mahjong.0x9.pw/" target=”_blank”> まーじゃん </a>
          </v-layout>  
        </v-col>
        <v-col cols="12">
          <p class="subtitle" align="left"> 
            見るからに麻雀です。そうです。
          </p>
        </v-col>
      </v-row>
    </v-container>
  </v-app>
</template>

<style scoped>
.club-page {
  background: url('~assets/ep_naturalwhite.png') fixed repeat round;
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